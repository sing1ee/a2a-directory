---
title: "A2A Sample Methods and JSON Responses"
date: "2024-04-12"
excerpt: "Explore comprehensive examples of A2A Protocol's core methods, including task management, streaming support, and structured data handling with detailed JSON responses."
metadata:
  title: "A2A Sample Methods and JSON Responses"
  description: "Detailed guide showcasing A2A Protocol's core methods, from basic task management to advanced features like streaming and structured data handling, with practical JSON examples."
  author: "A2A Team"
  image: "/a2a-sample.png"
---

## A2A Sample Methods and JSON Responses

### Agent Card
```json
{
"name": "Google Maps Agent",
"description": "Plan routes, remember places, and generate directions",
"url": "https://maps-agent.google.com",
"provider": {
  "organization": "Google",
  "url": "https://google.com"
},
"version": "1.0.0",
"authentication": {
  "schemes": "OAuth2"
},
"defaultInputModes": ["text/plain"],
"defaultOutputModes": ["text/plain", "application/html"],
"capabilities": {
  "streaming": true,
  "pushNotifications": false
},
"skills": [
  {
    "id": "route-planner",
    "name": "Route planning",
    "description": "Helps plan routing between two locations",
    "tags": ["maps", "routing", "navigation"],
    "examples": [
      "plan my route from Sunnyvale to Mountain View",
      "what's the commute time from Sunnyvale to San Francisco at 9AM",
      "create turn by turn directions from Sunnyvale to Mountain View"
    ],
    "outputModes": ["application/html", "video/mp4"]
  },
  {
    "id": "custom-map",
    "name": "My Map",
    "description": "Manage a custom map with your own saved places",
    "tags": ["custom-map", "saved-places"],
    "examples": [
      "show me my favorite restaurants on the map",
      "create a visual of all places I've visited in the past year"
    ],
    "outputModes": ["application/html"]
  }
]
}
```

### Send a Task
Allows a client to send content to a remote agent to start a new Task, resume an interrupted Task, or reopen a completed Task. A Task interrupt may be caused due to an agent requiring additional user input or a runtime error.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/send",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "tell me a joke"
      }
    ]
  },
  "metadata": {}
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "completed"
  },
  "artifacts": [
    {
      "name": "joke",
      "parts": [
        {
          "kind": "text",
          "text": "Why did the chicken cross the road? To get to the other side!"
        }
      ]
    }
  ],
  "metadata": {}
}
}
```

### Get a Task
Clients may use this method to retrieve the generated artifacts for a Task. The agent determines the retention window for Tasks previously submitted to it.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/get",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "historyLength": 10,
  "metadata": {}
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "completed"
  },
  "artifacts": [
    {
      "parts": [
        {
          "kind": "text",
          "text": "Why did the chicken cross the road? To get to the other side!"
        }
      ]
    }
  ],
  "history": [
    {
      "role": "user",
      "parts": [
        {
          "kind": "text",
          "text": "tell me a joke"
        }
      ]
    }
  ],
  "metadata": {}
}
}
```

### Cancel a Task
A client may choose to cancel previously submitted Tasks.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/cancel",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "metadata": {}
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": 1,
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "canceled"
  },
  "metadata": {}
}
}
```

### Set Task Push Notifications
Clients may configure a push notification URL for receiving an update on Task status change.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/pushNotification/set",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "pushNotificationConfig": {
    "url": "https://example.com/callback",
    "authentication": {
      "schemes": ["jwt"]
    }
  }
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "pushNotificationConfig": {
    "url": "https://example.com/callback",
    "authentication": {
      "schemes": ["jwt"]
    }
  }
}
}
```

### Get Task Push Notifications
Clients may retrieve the currently configured push notification configuration for a Task using this method.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/pushNotification/get",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64"
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "pushNotificationConfig": {
    "url": "https://example.com/callback",
    "authentication": {
      "schemes": ["jwt"]
    }
  }
}
}
```

### Multi-turn Conversations
A Task may pause to be executed on the remote agent if it requires additional user input.

#### Request - seq 1
```json
{
"jsonrpc": "2.0",
"id": 1,
"method": "tasks/send",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "request a new phone for me"
      }
    ]
  },
  "metadata": {}
}
}
```

#### Response - seq 2
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "input-required",
    "message": {
      "parts": [
        {
          "kind": "text",
          "text": "Select a phone type (iPhone/Android)"
        }
      ]
    }
  },
  "metadata": {}
}
}
```

#### Request - seq 3
```json
{
"jsonrpc": "2.0",
"id": 2,
"method": "tasks/send",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "Android"
      }
    ]
  },
  "metadata": {}
}
}
```

#### Response - seq 4
```json
{
"jsonrpc": "2.0",
"id": 2,
"result": {
  "id": 1,
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "completed"
  },
  "artifacts": [
    {
      "name": "order-confirmation",
      "parts": [
        {
          "kind": "text",
          "text": "I have ordered a new Android device for you. Your request number is R12443"
        }
      ],
      "metadata": {}
    }
  ],
  "metadata": {}
}
}
```

### Streaming Support
For clients and remote agents capable of communicating over HTTP with SSE, clients can send the RPC request with method `tasks/sendSubscribe` when creating a new Task.

#### Request
```json
{
"method": "tasks/sendSubscribe",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "write a long paper describing the attached pictures"
      },
      {
        "kind": "file",
        "file": {
          "mimeType": "image/png",
          "data": "<base64-encoded-content>"
        }
      }
    ]
  },
  "metadata": {}
}
}
```

#### Example Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": 1,
  "status": {
    "state": "working",
    "timestamp": "2025-04-02T16:59:25.331844"
  },
  "final": false
}
}
```

### Resubscribe to Task
A disconnected client may resubscribe to a remote agent that supports streaming to receive Task updates via SSE.

#### Request
```json
{
"method": "tasks/resubscribe",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "metadata": {}
}
}
```

#### Example Response
```json
{
"jsonrpc": "2.0",
"id": 1,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "artifact": [
    {
      "parts": [
        {
          "kind": "text",
          "text": "<section 2...>"
        }
      ],
      "index": 0,
      "append": true,
      "lastChunk": false
    }
  ]
}
}
```

### Non-textual Media
Following is an example interaction between a client and an agent with non-textual data.

#### Request - seq 1
```json
{
"jsonrpc": "2.0",
"id": 9,
"method": "tasks/send",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "Analyze the attached report and generate high level overview"
      },
      {
        "kind": "file",
        "file": {
          "mimeType": "application/pdf",
          "data": "<base64-encoded-content>"
        }
      }
    ]
  },
  "metadata": {}
}
}
```

#### Response - seq 2
```json
{
"jsonrpc": "2.0",
"id": 9,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "working",
    "message": {
      "role": "agent",
      "parts": [
        {
          "kind": "text",
          "text": "analysis in progress, please wait"
        }
      ],
      "metadata": {}
    }
  },
  "metadata": {}
}
}
```

#### Request - seq 3
```json
{
"jsonrpc": "2.0",
"id": 10,
"method": "tasks/get",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "metadata": {}
}
}
```

#### Response - seq 4
```json
{
"jsonrpc": "2.0",
"id": 9,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "completed"
  },
  "artifacts": [
    {
      "parts": [
        {
          "kind": "text",
          "text": "<generated analysis content>"
        }
      ],
      "metadata": {}
    }
  ],
  "metadata": {}
}
}
```

### Structured Output
Both the client or the agent can request structured output from the other party.

#### Request
```json
{
"jsonrpc": "2.0",
"id": 9,
"method": "tasks/send",
"params": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "message": {
    "role": "user",
    "parts": [
      {
        "kind": "text",
        "text": "Show me a list of my open IT tickets",
        "metadata": {
          "mimeType": "application/json",
          "schema": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "ticketNumber": { "type": "string" },
                "description": { "type": "string" }
              }
            }
          }
        }
      }
    ]
  },
  "metadata": {}
}
}
```

#### Response
```json
{
"jsonrpc": "2.0",
"id": 9,
"result": {
  "id": "de38c76d-d54c-436c-8b9f-4c2703648d64",
  "sessionId": "c295ea44-7543-4f78-b524-7a38915ad6e4",
  "status": {
    "state": "working",
    "message": {
      "role": "agent",
      "parts": [
        {
          "kind": "text",
          "text": "[{\"ticketNumber\":\"REQ12312\",\"description\":\"request for VPN access\"},{\"ticketNumber\":\"REQ23422\",\"description\":\"Add to DL - team-gcp-onboarding\"}]"
        }
      ],
      "metadata": {}
    }
  },
  "metadata": {}
}
}
```