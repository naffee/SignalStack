---
layout: default
title: Migration Guide
nav_order: 4
permalink: /migration-guide/
---

# Migration Guide: v1.0 → v2.0

This guide will help you upgrade your integration from SignalStack v1.0 to v2.0.

## Overview

Version 2.0 introduces a new SDK and improved API structure. While the core concepts remain the same, there are some breaking changes you need to be aware of.

## Breaking Changes

### SDK Import
The SDK package name has changed.

**v1.0**
```javascript
const SignalStack = require('signalstack-v1');
```

**v2.0**
```javascript
import { SignalStackClient } from 'signalstack-v2';
```

### Authentication
API Keys are now passed in a configuration object, not as a direct string argument.

**v1.0**
```javascript
const client = new SignalStack('MY_KEY');
```

**v2.0**
```javascript
const client = new SignalStackClient({ apiKey: 'MY_KEY' });
```

## Deprecated Features

- **Basic Triggers**: The "Triggers" tab in the dashboard has been replaced by "Routing Rules". Your existing triggers have been automatically migrated to simple rules.

## Step-by-Step Upgrade

1. Update your dependency to `signalstack-v2`.
2. Update your client initialization code.
3. Verify your event payloads match the v2 schema (mostly backward compatible).
4. Test your integration in the sandbox environment.
