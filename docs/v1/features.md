---
layout: default
title: Features
parent: Version 1.0
nav_order: 2
permalink: /docs/v1/features/
---

# Features (v1.0)

## Event Dispatching

SignalStack v1.0 provides robust event dispatching capabilities. You can emit events from your application and have them delivered to configured endpoints.

### Supported Protocols

- HTTP/HTTPS Webhooks

## Webhook Delivery

Webhooks are delivered via POST requests with a JSON payload.

### Payload Structure

```json
{
  "event": "user.signup",
  "timestamp": "2023-10-27T10:00:00Z",
  "data": {
    "userId": "12345",
    "email": "user@example.com"
  }
}
```

## Basic Triggers

Configure triggers in the dashboard to listen for specific event types and fire webhooks. Currently supports exact match on event names.
