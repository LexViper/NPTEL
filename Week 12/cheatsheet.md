# Week 12 Cheat Sheet: NPTEL Cloud Computing

## Exam Context
- **100-mark MCQ Exam**: 12 weeks, ~8-10 marks for Week 12 (8-10 questions).
- **Topics**: Cloud Computing in 5G Era, Cyber-Physical Systems (CPS), Spatial Cloud Computing, Internet of Health Things (IoHT).
- **MCQ Types**: Definitions (e.g., 5G vs. 4G), comparisons (e.g., cloud vs. fog), scenarios (e.g., CPS applications), numericals (e.g., IoHT latency, bandwidth).
- **Prep Tips**:
  - Memorize mnemonics for key features and frameworks.
  - Focus on high-yield topics: 5G features, CPS components, spatial cloud advantages, IoHT fog-edge benefits.
  - Practice quick comparisons (e.g., cloud vs. fog vs. dew).
  - Time: ~1.2 min/question, skip complex ones initially.

---

## 1. Cloud Computing in 5G Era

### Theory
- **5G Overview**: 5th generation mobile network, connects everything (machines, IoT, devices) with high speeds (>10 Gbps), low latency (<1ms), and massive capacity.
- **5G Features**:
  - **eMBB**: Enhanced mobile broadband (VR, AR).
  - **mMTC**: Massive IoT (smart cities, sensors).
  - **URLLC**: Ultra-reliable low-latency (autonomous vehicles, telehealth).
- **Cloud + 5G**:
  - Edge/fog computing reduces latency.
  - Cloudification via NFV, SDN.
  - Network as a Platform for enterprise services.
- **Edge Computing**: Brings cloud capabilities near users, supports AR/VR, IoT.

**Mnemonic**: **5G = Speedy, Global, Gadget-Grid** (Speedy for Gbps, Global for connectivity, Gadget-Grid for IoT).

### MCQ Tips
- **Evolution**: 1G (analog voice), 2G (digital), 3G (data), 4G (broadband), 5G (hyperconnectivity).
- **Features**: eMBB (VR), mMTC (IoT), URLLC (vehicles).
- **Cloud Role**: Edge for latency, NFV/SDN for cloudification.
- **Numericals**: Compare latency (5G <1ms vs. 4G 60-98ms).

**Example MCQ**:
- **Q**: 5G latency compared to 4G?
  - **A**: <1ms (4G: 60-98ms).

---

## 2. Cyber-Physical Systems (CPS)

### Theory
- **Definition**: Integration of computation, physical processes, and communication via sensors/actuators with feedback loops.
- **Components**: Cyber (computing), Physical (environment), Sensors/Actuators, Feedback.
- **Applications**: Smart grid, autonomous vehicles, medical devices, robotics.
- **CPS + Cloud**: Cyber-Physical Cloud Computing (CPCC) framework for scalable, modular, resilient systems.
- **CPCC Benefits**: Resource efficiency, rapid development, smart adaptation.

**Mnemonic**: **CPS = Compute, Physical, Sense-Act** (Compute for cyber, Physical for environment, Sense-Act for sensors/actuators).

### MCQ Tips
- **Definition**: CPS = cyber + physical integration, not union.
- **Applications**: Focus on smart grid, vehicles, healthcare.
- **CPCC**: Scalability, modularity.
- **Scenario**: Identify CPS examples (e.g., robotics vs. pure software).

**Example MCQ**:
- **Q**: CPS example?
  - **A**: Smart grid (integrates computing + physical).

---

## 3. Spatial Cloud Computing

### Theory
- **Spatial Data**: Geospatial info (location + attributes + time).
- **Spatial Analysis**: Solves location-oriented problems (e.g., crime mapping, drought analysis).
- **Spatial Cloud**: Cloud platform for geospatial data, supports scalability, shared resources.
- **Advantages**: Easy deployment, cost-optimized, reliable, scalable.
- **Traj-Cloud**: Analyzes mobility traces (e.g., GPS, IoT) for urban dynamics, ITS.
- **Traj-Cloud Services**: Indexing (TS1), Map-matching (TS2), Query (TS3).

**Mnemonic**: **SPATIAL = Scalable Platform for Analysis, Trajectories, and Intelligent Applications of Location**.

### MCQ Tips
- **Data**: Location + attributes + time.
- **Advantages**: Scalability, cost.
- **Traj-Cloud**: Services (TS1-TS3), urban dynamics.
- **Scenario**: Spatial vs. non-spatial (e.g., crime mapping vs-std database).

**Example MCQ**:
- **Q**: Traj-Cloud service for GPS indexing?
  - **A**: TS1 (Trajectory Indexing).

---

## 4. Internet of Health Things (IoHT)

### Theory
- **IoHT**: IoT for healthcare (wearables, sensors).
- **Cloud-Fog-Edge Framework**:
  - **Cloud**: Big data, storage.
  - **Fog**: Local processing, low latency.
  - **Edge**: Real-time data from sensors.
  - **Dew**: On-premises, independent + cloud-collaborative.
- **Objectives**: Reduce latency, network usage, cloud costs.
- **Case Study**: Fog-edge model for cardiac attack prediction (BPM ≥170, systolic ≥180, diastolic ≥120).
- **Performance**:
  - Fog: Lower latency, network usage, cost.
  - Cloud: Higher latency, cost.
- **Tools**: iFogSim (simulation), NodeMCU, Raspberry Pi (hardware).

**Mnemonic**: **IoHT = Intelligent, On-site Health Tech** (Intelligent for analytics, On-site for fog/edge, Health Tech for IoT).

### MCQ Tips
- **Framework**: Cloud (storage), Fog (processing), Edge (sensors), Dew (on-premises).
- **Performance**: Fog > Cloud for latency, cost.
- **Case Study**: Cardiac thresholds, iFogSim.
- **Numericals**: Latency (e.g., fog = 100ms vs. cloud = 500ms).

**Example MCQ**:
- **Q**: IoHT fog model advantage?
  - **A**: Low latency (vs. cloud).

---

## Quick Revision Checklist
- **5G**: eMBB, mMTC, URLLC; edge for latency.
- **CPS**: Cyber + physical; CPCC for scalability.
- **Spatial Cloud**: Scalability, Traj-Cloud (TS1-TS3).
- **IoHT**: Fog-edge for low latency; cardiac thresholds.
- **Practice**: 5-10 MCQs/day, focus on comparisons.