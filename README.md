# Tenable_OT_Exposure_For_Splunk_App
Tenable OT Exposure for Splunk App



- Tenable OT Exposure is a very complex solution especially reverse engineering for an Executive At a Glance standalone Splunk Application


## 🏗️ Intended Use Cases

- OT Asset Inventory Export
- Sensor Health Auditing
- OT Event Analysis
- Vulnerability & Plugin Risk Analysis
- IoT/OT discovery, identification, classification mapping based on multiple asset attributes not IP address
- SIEM / Data Lake Ingestion (tool-agnostic)

⚠️ Disclaimer



- GraphQL API for Tenable OT is poorly documented, it takes years to master GraphQL Schema archaeology + API reconstruction + OT domain modeling then apply that to Tenable's attempt after Indegy ICS acquisition where most Enterprises will leverage less than 1% of the API capabilities

- The User Interface is not designed for large scale administration for asset owners, no operational management for operational utilization, health, user monitoring, activity day over day, week over week, month over month, quarter over quarter, year over year.
- 
- No User Access Reviews, No Asset fatigure review, no Policy fatigure is covered.
  



## Skills Required

- Years of Extensive GraphQL Experience

- Years of schema design and harvesting

- Years of reverse-engineering/reverse mapping to provide Executive Level, Senior Management, Asset Custodians at a glance Visualizations without requiring access to the TenableOne or TenableOT Platform.

- Schema-first thinking (types, enums, connections, edges)

- Cursor-based pagination (not offset-based)

- How enums actually constrain valid queries

- How permissions and capabilities gate fields are implemented

- How vendor-specific modeling choices work

⚠️ Disclaimer


Use of this package are not covered by any license, warranty, or support agreement you may have with Tenable.
All functionality is implemented independently using publicly available Tenable OT Exposure API documentation.



## 🚀 Key Capabilities

### 🧠 OT Asset Intelligence
| Feature | Description |
|------|-------------|
| 🏗️ Asset Inventory | Full OT asset extraction including type, vendor, firmware, serial, OS, Purdue level |
| 🧬 Asset Classification | Asset types, categories, roles, safety-rated flags |
| 🌐 Network Context | IPs, MACs, VLANs, segments, zones |
| 🧱 Purdue Model Mapping | Native Purdue level support (L0–L5) |
| ⏱️ Lifecycle Visibility | First seen, last seen, update timestamps |
| 🧾 Revision Tracking | Asset revisions and configuration changes |

---

### 🔍 Detection & Risk Analytics
| Feature | Description |
|------|-------------|
| 🚨 OT Events | Security, policy, and operational events |
| 📊 Aggregated Event Metrics | 24h / 7d / 30d event aggregation |
| ⚠️ Severity & Category | Event severity, family, category, protocol |
| 🧩 Policy Context | Event-to-policy attribution |
| 🔄 Continuous vs Snapshot | Supports both continuous and snapshot detections |

---

### 🛡️ Vulnerability & Plugin Intelligence
| Feature | Description |
|------|-------------|
| 🔌 OT Plugins | Plugin metadata, source, family, severity |
| 📈 Risk Metrics | VPR, CVSS, unresolved events |
| 🧠 Asset Enrichment | Extended plugin details and references |
| 🔗 Asset Impact | Plugin-to-asset relationships |

---

### 🛰️ Sensor & Infrastructure Health
| Feature | Description |
|------|-------------|
| 📡 ICP Sensor Status | Sensor connectivity, health, last seen |
| 🧭 Sensor Types | Component and protocol-specific sensors |
| 🧪 BACnet & OT Protocol Visibility | BACnet object types, protocol metadata |
| 🕒 Telemetry Timelines | Time-based operational metrics |

---

### 👥 User & Access Intelligence
| Feature | Description |
|------|-------------|
| 👤 Users | User accounts and roles |
| 🔑 Authentication Validation | GraphQL-based API key verification |
| 🧾 User Activity | Action types, policy interactions |
| 🔍 User Visibility | User-driven operational actions |

---


## 🧱 Architecture Highlights

| Component | Purpose |
|--------|--------|
| 🧠 GraphQL Templates | Schema-aligned queries |
| 🔁 Pagination Engine | Cursor-based extraction |
| 🧪 Validation Layer | API key and permission validation |
| 📦 Export Formats | JSON and CSV ready |
| ⏱️ Rate Control | Retry, backoff, and timeout discipline |
| 🧯 Error Normalization | Structured failure events |

---

## 🎯 Design Principles

- ✅ **Schema-First** – Queries align exactly with Tenable OT Exposure documentation 
- 🔒 **Safe by Default** – Read-only GraphQL operations only  
- 🧪 **Validated** – Designed to run in GraphiQL Playground  
- 🧩 **Composable** – Each query stands alone  

---

## 🧪 Validation & Testing

- Tested using Tenable OT Exposure **GraphiQL Playground**
- Supports cursor-based pagination
- Handles empty result sets gracefully
- Validates API access before extraction

---



---

## 📚 References

- Tenable OT Exposure GraphQL Playground  
  https://developer.tenable.com/docs/ot-graphiql-playground

- Tenable OT Exposure API Documentation  
  https://docs.tenable.com/OT-security/api/

---

	

