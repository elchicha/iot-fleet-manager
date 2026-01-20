# Architecture Overview

## Systems Design Philosophy

This IoT platform is designed with enterprise-grade patterns to demonstrate:
- **Scalability** - Handle thousands of simulated devices
- **Resiliency** - Graceful degradation and error handling
- **Observability** - Full visibility into system behavior
- **Maintainability** - Clear separation of concerns
- **Extensibility** - Easy to add new device types and features

## High-Level Architecture
```
┌─────────────────┐
│ Simulated       │
│ IoT Devices     │ (Python scripts)
└────────┬────────┘
         │ MQTT
         ↓
┌─────────────────┐
│ MQTT Broker     │ (Mosquitto)
│ (Message Bus)   │
└────────┬────────┘
         │
         ↓
┌─────────────────┐      ┌──────────────┐
│ Device Manager  │◄────►│ PostgreSQL   │
│ API (FastAPI)   │      │ + TimescaleDB│
└────────┬────────┘      └──────────────┘
         │
         ├─► WebSocket → Dashboard
         ├─► REST API → External Clients
         └─► Background Tasks → Rule Engine
```