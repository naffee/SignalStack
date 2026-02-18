---
layout: default
title: Changelog
nav_order: 3
permalink: /changelog/
---

# Changelog

All notable changes to SignalStack will be documented in this file.

## [2.0.0] - 2023-11-15

### Added
- **Smart Event Routing**: Dynamic routing based on payload.
- **Retry Engine**: Configurable retry policies with exponential backoff.
- **Advanced Analytics**: Real-time insights dashboard.

### Changed
- **SDK**: Complete rewrite of Node.js SDK (`signalstack-v2`).
- **API**: Standardized response format for all endpoints.

### Deprecated
- **v1 SDK**: `signalstack-v1` is now in maintenance mode.
- **Basic Triggers**: Replaced by Smart Routing rules.

## [1.1.0] - 2023-08-01

### Added
- Webhook signature verification.
- Improved error messages.

## [1.0.0] - 2023-01-10

### Initial Release
- Core Event Dispatching.
- Basic Webhook Support.
