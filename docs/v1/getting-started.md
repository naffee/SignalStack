---
layout: default
title: Getting Started
parent: Version 1.0
nav_order: 1
permalink: /docs/v1/getting-started/
---

# Getting Started with v1.0

Follow these steps to integrate SignalStack v1.0 into your application.

## Prerequisites

- Ensure you have an active SignalStack account.
- Obtain your API Key from the dashboard.

## Installation

Install the SignalStack client library:

```bash
npm install signalstack-v1
```

## Basic Usage

Initialize the client and emit an event:

```javascript
const SignalStack = require('signalstack-v1');
const client = new SignalStack('YOUR_API_KEY');

client.emit('user.signup', {
  userId: '12345',
  email: 'user@example.com'
});
```

This will trigger any webhooks configured for the `user.signup` event.
