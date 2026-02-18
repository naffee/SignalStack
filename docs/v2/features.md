---
layout: default
title: Features
parent: Version 2.0
nav_order: 2
permalink: /docs/v2/features/
---

# New Features in v2.0

SignalStack v2.0 introduces powerful new capabilities to manage your event streams.

## Smart Event Routing

Route events to specific endpoints based on payload content. Define routing rules in the dashboard or via API.

- **Example**: Route `priority: "high"` events to a dedicated fast-lane webhook.

## Retry Engine

Configure automatic retry policies for failed deliveries.

- **Exponential Backoff**: Inteligently wait between retry attempts.
- **Dead Letter Queues**: Capture events that fail after max retries for manual inspection.

## Advanced Analytics

Real-time visibility into your event pipeline.

- **Delivery Success Rate**: Track % of successful deliveries.
- **Latency Metrics**: Monitor end-to-end delivery time.

## Event Filtering

Filter events at the source before they are dispatched, saving bandwidth and processing power.
