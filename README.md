# IoT Fleet Manager 

> Enterprise-grade IoT device management platform demonstrating distributed systems architecture, event-driven design, and edge computing patterns.


[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)


## Overview

A fully simulated IoT platform built to demonstrate enterprise architecture patterns for managing fleets of connected devices.
This project showcases scalable, resilient distributed systems design suitable for production IoT deployments.

## 🏗️ Architecture

High-level system design:
```
[Simulated Devices] → [MQTT Broker] → [Device Manager API] → [PostgreSQL]
                           ↓                    ↓
                    [Rule Engine]        [WebSocket]
                           ↓                    ↓
                      [Alerts]           [Dashboard]
```


## ✨ Features

### Current
- ✅ Project structure and documentation

### Planned
- [ ] Simulated IoT devices with realistic telemetry
- [ ] MQTT pub/sub messaging
- [ ] Device registration and management API
- [ ] Real-time telemetry storage
- [ ] Device shadow (digital twin) pattern
- [ ] Command & control system
- [ ] Rule-based alerting engine
- [ ] Real-time web dashboard
- [ ] Edge gateway simulation
- [ ] Observability (metrics, logs, traces)