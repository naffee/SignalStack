---
layout: default
title: Getting Started
parent: Version 2.0
nav_order: 1
permalink: /docs/v2/getting-started/
---

# Getting Started with v2.0 (Latest)

Welcome to SignalStack v2.0! This guide will help you get up and running with the latest features.

## Prerequisites

- **New Requirement**: Node.js 18+ environment (v2 SDK requirement).
- existing SignalStack account.

## Installation

Install the new v2 SDK:

```bash
npm install signalstack-v2
```

## Quick Start

Initialize the client with enhanced configuration options:

```javascript
import { SignalStackClient } from 'signalstack-v2';

const client = new SignalStackClient({
  apiKey: process.env.SIGNALSTACK_API_KEY,
  options: {
    retry: true, // Enable automatic retries
    timeout: 5000 // 5s timeout
  }
});

await client.events.emit('order.created', {
  orderId: '98765',
  amount: 49.99
});
```

See [Migration Guide](../../migration-guide.html) if upgrading from v1.
