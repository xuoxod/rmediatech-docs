# RMEDIATECH SYSTEMS ARSENAL SPECIFICATION

- **Namespace**: `rmt::arsenal::specification`
- **Classification**: Public Technical Architecture Guide
- **Revision**: 2026.1

---

## 1. Overview of Companion Utilities

The RMediaTech platform provides a curated arsenal of high-assurance companion utilities designed for rapid deployment on edge Linux systems. Each tool is compiled as a static, self-contained executable that can be installed on bare-metal systems with zero library dependencies.

---

## 2. Utility Registry & Functional Roles

### 2.1 Bastion (`rmt::tool::bastion`)
- **Primary Function**: Tactical Network Reconnaissance & L2/L4 Boundary Verification
- **Operational Scope**: Host discovery, Layer 4 TCP sweeping, wireless airspace inspection, and structured forensic reporting.
- **Output Artifacts**: Normalized JSON/CSV forensic event reports.

### 2.2 Conduit (`rmt::tool::conduit`)
- **Primary Function**: Sovereign Zero-Trust Bridge & Edge Tunneling Engine
- **Operational Scope**: Secure peer-to-peer interconnectivity across network enclaves, NAT traversal, and outpost communication without exposing public listener ports.

### 2.3 Forgetunnel (`rmt::tool::forgetunnel`)
- **Primary Function**: Ephemeral Privacy-Preserving Proxy Routing
- **Operational Scope**: On-demand outbound traffic routing, encrypted forwarding, and volatile connection teardown.

### 2.4 Nexus-Recon (`rmt::tool::nexus_recon`)
- **Primary Function**: High-Speed Cluster Node Discovery & Service Inspection
- **Operational Scope**: Fast network mapping, socket availability auditing, and boundary diagnostic logs.

### 2.5 Sentry-Edge (`rmt::tool::sentry_edge`)
- **Primary Function**: Perimeter Telemetry Sentinel & Anomaly Detection
- **Operational Scope**: Real-time traffic monitoring, threshold-based heuristic alert dispatch, and continuous host environment telemetry.

### 2.6 Sovereign-Ledger (`rmt::tool::sovereign_ledger`)
- **Primary Function**: Verifiable Local Audit Trail & Event Serialization
- **Operational Scope**: Tamper-evident forensic activity recording and sequential audit verification.

### 2.7 RMailer (`rmt::tool::rmailer`)
- **Primary Function**: Autonomous Transactional Email Dispatcher
- **Operational Scope**: Tracker-free, privacy-preserving transactional communications, password recovery delivery, and administrative alerts.

### 2.8 Ostium (`rmt::tool::ostium`)
- **Primary Function**: Autonomous Gateway Sentinel & Wardriving Defense (WIDS)
- **Operational Scope**: Qualcomm QSDK hardware fingerprinter, 802.11w WIDS wardriving defense platform, and autonomous perimeter breach monitoring.

---

## 3. Distribution Standard

All companion binaries adhere to the **Sovereign Musl Standard**:
- Built against `x86_64-unknown-linux-musl`
- Zero external runtime library linkages (`ldd` returns `not a dynamic executable`)
- Verifiable cryptographic checksums (SHA-256) distributed with each artifact
- Single-command streaming installer scripts served directly from the native web platform

---

&copy; 2026 RMediaTech. All Rights Reserved. Sovereign Edge Platform.
