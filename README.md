# iot-fleet-manager
Enterprise-grade IoT device management platform with edge computing simulation

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