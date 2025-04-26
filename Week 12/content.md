# Week 12 Complete Guide: NPTEL Cloud Computing

## Exam Context
- **100-mark MCQ Exam**: 12 weeks, ~8-10 marks for Week 12 (8-10 questions).
- **Topics**: Cloud Computing in 5G Era, Cyber-Physical Systems (CPS), Spatial Cloud Computing, Internet of Health Things (IoHT).
- **MCQ Types**:
  - Definitions (e.g., 5G features, CPS vs. IoT).
  - Comparisons (e.g., cloud vs. fog vs. dew).
  - Scenarios (e.g., Traj-Cloud services, IoHT applications).
  - Numericals (e.g., latency, bandwidth, cost in IoHT).
- **Prep Strategy**:
  - Memorize mnemonics for frameworks, features.
  - Practice comparisons (e.g., 5G vs. 4G, fog vs. cloud).
  - Focus on numericals (latency, network usage).
  - Time: ~1.2 min/question, skip complex ones initially.
- **High-Yield Topics**:
  - 5G: eMBB, mMTC, URLLC (~2-3 MCQs).
  - CPS: CPCC, applications (~2 MCQs).
  - Spatial Cloud: Traj-Cloud, advantages (~2 MCQs).
  - IoHT: Fog-edge benefits, cardiac case (~2-3 MCQs).

---

## 1. Cloud Computing in 5G Era

### Theory
- **5G Definition**: 5th generation mobile network, succeeds 1G (analog voice, 1980s), 2G (digital voice, 1990s), 3G (mobile data, 2000s), 4G (broadband, 2010s). Connects machines, IoT, devices.
- **5G Features**:
  - **Peak Speed**: >10 Gbps (4G: 10 Gbps).
  - **Latency**: <1ms (4G: 60-98ms).
  - **Capacity**: Massive IoT support.
  - **Reliability**: Ultra-reliable for mission-critical apps.
- **Service Types**:
  - **eMBB**: Enhanced mobile broadband (VR, AR, enterprise).
  - **mMTC**: Massive machine-type communications (IoT, smart cities).
  - **URLLC**: Ultra-reliable low-latency (autonomous vehicles, telehealth).
- **5G + Cloud**:
  - **Edge Computing**: Reduces latency for AR/VR, IoT.
  - **Cloudification**: NFV (Network Function Virtualization), SDN (Software-Defined Networking).
  - **Network as a Platform**: Orchestrates enterprise services with QoS.
- **Applications**: Healthcare, entertainment, smart grids, ITS.

**Mnemonic**: **5G = Speedy, Global, Gadget-Grid** (Speedy for Gbps, Global for connectivity, Gadget-Grid for IoT).

### Evolution Table
| Generation | Decade | Speed | Latency | Feature |
|------------|--------|-------|---------|---------|
| 1G         | 1980s  | 2 kbps | N/A     | Analog voice |
| 2G         | 1990s  | 384 kbps | 629ms | Digital voice |
| 3G         | 2000s  | 56 Mbps | 212ms | Mobile data |
| 4G         | 2010s  | 10 Gbps | 60-98ms | Broadband |
| 5G         | 2020s  | >10 Gbps | <1ms | Hyperconnectivity |

### Mobile Cloud Computing (MCC)
- **Definition**: Cloud system delivering apps to mobile devices via 5G.
- **Features**: Resource sharing, offloads processing to cloud, improves reliability.
- **Benefit**: Reduces device resource usage.

### MCQ Strategies
- **Evolution**: Memorize speeds, latency (e.g., 5G <1ms).
- **Features**: eMBB (VR), mMTC (IoT), URLLC (vehicles).
- **Cloud Role**: Edge for latency, NFV/SDN for cloudification.
- **MCC**: Offloading, reliability.
- **Traps**: Confusing 4G/5G latency, mixing eMBB/mMTC.

**Practice MCQ**:
- **Q**: 5G feature for autonomous vehicles?
  - **A**: URLLC (ultra-reliable, low-latency).

---

## 2. Cyber-Physical Systems (CPS)

### Theory
- **Definition**: Integration of computation and physical processes via sensors/actuators with feedback loops (coined 2006, Helen Gill, NSF).
- **Components**:
  - **Cyber**: Computing, software.
  - **Physical**: Environment (e.g., vehicles, grids).
  - **Sensors/Actuators**: Monitor/control physical world.
  - **Feedback**: Physical affects cyber, vice versa.
- **Characteristics**: Multi-disciplinary (engineering + CS), operates on varied scales, context-dependent.
- **Applications**: Smart grid, autonomous vehicles, medical devices, robotics, industrial control.
- **CPS + Cloud**:
  - **Cyber-Physical Cloud Computing (CPCC)**: Framework for scalable, modular CPS.
  - **Smart Networked Systems and Societies (SNSS)**: Network of sensors, actuators, humans.
- **CPCC Benefits**:
  - Efficient resource use.
  - Modular composition.
  - Rapid development, scalability.
  - Smart adaptation.
  - Reliable, resilient architecture.

**Mnemonic**: **CPS = Compute, Physical, Sense-Act** (Compute for cyber, Physical for environment, Sense-Act for sensors/actuators).

### MCQ Strategies
- **Definition**: CPS = integration, not union.
- **Applications**: Smart grid, vehicles, healthcare.
- **CPCC**: Focus on scalability, modularity.
- **Scenario**: CPS vs. pure software (e.g., robotics = CPS).
- **Traps**: Mixing CPS with IoT (CPS includes physical feedback).

**Practice MCQ**:
- **Q**: CPCC benefit?
  - **A**: Scalability (rapid development).

---

## 3. Spatial Cloud Computing

### Theory
- **Spatial Data**: Geospatial info with location (coordinates), attributes (characteristics), and time.
- **Spatial Analysis**: Solves location-oriented problems (e.g., crime mapping, drought analysis, optimal paths).
- **Spatial Cloud**:
  - Cloud platform for geospatial data.
  - Supports shared resources, scalability, reliability.
- **Advantages**:
  - Easy deployment (click-based, API-driven).
  - Scalability (app-based infrastructure).
  - Cost-optimized (usage-based).
  - Reliability (enterprise-grade hardware).
  - Low risk (instant changes).
- **Architecture**:
  - **WPS**: Web Processing Service.
  - **CSW**: Catalogue Service for Web.
  - Integrates databases, disparate systems.
- **Traj-Cloud**:
  - Analyzes mobility traces (GPS, IoT) for urban dynamics, ITS.
  - **Services**:
    - **TS1**: Trajectory Indexing (BigQuery, Cloud SQL).
    - **TS2**: Map-matching (Compute Engine).
    - **TS3**: Query (Compute Engine, Cloud SQL).
- **Applications**: Crime studies, drought analysis, mobility analytics (human, animal, vehicles).

**Mnemonic**: **SPATIAL = Scalable Platform for Analysis, Trajectories, and Intelligent Applications of Location**.

### MCQ Strategies
- **Data**: Location + attributes + time.
- **Advantages**: Scalability, cost, reliability.
- **Traj-Cloud**: TS1 (indexing), TS2 (map-matching), TS3 (query).
- **Scenario**: Spatial (crime mapping) vs. non-spatial (database).
- **Traps**: Mixing TS1-TS3 functions, confusing spatial with temporal.

**Practice MCQ**:
- **Q**: Spatial cloud advantage?
  - **A**: Scalability (app-based infrastructure).

---

## 4. Internet of Health Things (IoHT)

### Theory
- **IoHT**: IoT for healthcare (wearables, sensors for health monitoring).
- **Cloud-Fog-Edge-Dew Framework**:
  - **Cloud**: Big data processing, storage.
  - **Fog**: Local processing (routers, servers), low latency.
  - **Edge**: Real-time data from sensors (wearables).
  - **Dew**: On-premises, independent + cloud-collaborative.
- **Objectives**:
  - Reduce latency, network usage, cloud costs.
  - Develop wearable devices for health parameters.
  - Test via iFogSim, hardware.
- **Case Study**: Cardiac attack prediction:
  - **Thresholds**: BPM ≥170, systolic ≥180, diastolic ≥120.
  - **Logic**: KNN classifier (K=3), accelerometer data.
  - **Hardware**: NodeMCU ESP8266, Raspberry Pi 3, BP/pulsemeter, ADXL345.
- **Performance** (Fog vs. Cloud):
  - **Latency**: Fog (low, ~100ms) vs. Cloud (high, ~500ms).
  - **Network Usage**: Fog (low, only confirmatory module on cloud) vs. Cloud (high, all modules on cloud).
  - **Cost**: Fog (low, owned resources) vs. Cloud (high, cloud processing).
- **Dew Benefits**: Optimal on-premise resource use, low bandwidth/latency.

**Mnemonic**: **IoHT = Intelligent

, On-site Health Tech** (Intelligent for analytics, On-site for fog/edge, Health Tech for IoT).

### Configuration (Fog-Edge)
| Device | MIPS | RAM (MB) | Up Bw (Kbps) | Down Bw (Kbps) | Level | Cost/MIPS |
|--------|------|----------|--------------|----------------|-------|-----------|
| Cloud  | 44800| 40000    | 100          | 10000          | 0     | 0.01      |
| ISP    | 2800 | 4000     | 10000        | 10000          | 1     | 0         |
| AreaGW | 2800 | 4000     | 10000        | 10000          | 2     | 0         |
| Mobile | 350  | 1000     | 10000        | 270            | 3     | -         |

**Latency**:
| Source       | Destination | Latency (ms) |
|--------------|-------------|--------------|
| Body sensor  | Mobile      | 1            |
| Mobile       | Area GW     | 2            |
| Area GW      | ISP GW      | 2            |
| ISP GW       | Cloud       | 100          |
| Mobile       | Display     | 1            |

### Numerical Example
**Q**: Fog model, control loop involves Mobile → Area GW → Mobile. Latency?

**Solution**:
1. Mobile → Area GW: 2ms.
2. Area GW → Mobile: 2ms (assume symmetric).
3. Total: 2 + 2 = **4ms**.

### MCQ Strategies
- **Framework**: Cloud (storage), Fog (processing), Edge (sensors), Dew (on-premises).
- **Performance**: Fog > Cloud for latency, cost, network.
- **Case Study**: Cardiac thresholds (BPM ≥170), iFogSim.
- **Numericals**: Latency (fog vs. cloud), bandwidth.
- **Traps**: Mixing fog/edge roles, incorrect thresholds.

**Practice MCQ**:
- **Q**: IoHT fog model latency for Mobile → Area GW?
  - **A**: 2ms (per table).

---

## Quick Revision Checklist
### Key Concepts
- **5G**: eMBB (VR), mMTC (IoT), URLLC (vehicles); edge for latency.
- **CPS**: Cyber + physical; CPCC for scalability.
- **Spatial Cloud**: Scalability, Traj-Cloud (TS1-TS3).
- **IoHT**: Fog-edge for low latency; cardiac thresholds (BPM ≥170).

### Mnemonics
- **5G**: Speedy, Global, Gadget-Grid.
- **CPS**: Compute, Physical, Sense-Act.
- **SPATIAL**: Scalable Platform for Analysis, Trajectories, and Intelligent Applications of Location.
- **IoHT**: Intelligent, On-site Health Tech.

### Shortcuts
- **5G**: Latency <1ms, speed >10 Gbps.
- **CPS**: Focus on feedback loops.
- **Spatial**: TS1 (index), TS2 (map), TS3 (query).
- **IoHT**: Fog = low latency (~4ms), cloud = high (~100ms).

### Practice MCQs
1. **5G**:
   - **Q**: 5G application for smart cities?
     - **A**: mMTC (massive IoT).
2. **CPS**:
   - **Q**: CPS component?
     - **A**: Sensors (monitor physical world).
3. **Spatial Cloud**:
   - **Q**: Traj-Cloud service for map-matching?
     - **A**: TS2 (Map-matching).
4. **IoHT**:
   - **Q**: Cardiac attack threshold for systolic?
     - **A**: ≥180.

---

## Exam Tips
- **Comparisons**: Cloud vs. fog vs. dew (latency, bandwidth).
- **Numericals**: Latency (fog = low, cloud = high), bandwidth.
- **Traps**: Mixing 5G features (eMBB vs. URLLC), IoHT thresholds.
- **Practice**: 5-10 MCQs daily, focus on fog-edge benefits.