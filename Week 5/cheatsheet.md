Below is the raw Markdown code for the NPTEL Cloud Computing Week 5 Cheat Sheet, fully formatted with proper headings, subheadings, code blocks for formulas, highlighted mnemonics, clean spacing, and a **Table of Contents** with clickable links. This is ready to be copied into a `.md` file (e.g., `nptel_cloud_computing_week5_cheatsheet.md`) and uploaded to GitHub.


# NPTEL Cloud Computing Week 5 Cheat Sheet

**A concise, exam-focused cheat sheet for Week 5 numericals and concepts, designed for NPTEL Cloud Computing MCQs. Perfect for rapid revision!**

---

## Table of Contents
- [Exam Context](#exam-context)
- [1. Service Level Agreements (SLAs)](#1-service-level-agreements-slas)
- [2. Cloud Economics](#2-cloud-economics)
- [3. MapReduce](#3-mapreduce)
- [4. Resource Management - I](#4-resource-management---i)
- [Quick Revision Checklist](#quick-revision-checklist)

---

## Exam Context

- **100-mark MCQ Exam** (12 weeks total)
- **~8–10 marks** from Week 5 (~8–10 questions)
- **Topics Covered**:
  - Service Level Agreements (SLAs)
  - Cloud Economics
  - MapReduce
  - Resource Management
- **MCQ Types**:
  - Definitions
  - Calculations (e.g., downtime, costs)
  - Scenarios (e.g., MapReduce phases)
  - Comparisons (cloud vs. in-house)

### Prep Tips
- Memorize **mnemonics** for formulas and concepts.
- Practice quick calculations (percentages, integrals, ceiling functions).
- Focus on high-yield topics: SLA violations, utility pricing, MapReduce phases.

---

## 1. Service Level Agreements (SLAs)

### Theory
- **Definition**: Contract between Service Provider (SP) and Service Consumer (SC) guaranteeing performance/availability.
- **Service Level Objectives (SLOs)**: Measurable metrics (e.g., 99.9% uptime, <5ms latency).
- **Purpose**: Builds trust, aids provider selection.
- **Service Credits**: Compensation for SLA violations (e.g., 10% for <99.95%, 25% for <99%).

### Mnemonic
**_SLA = Surety, Levels, Accountability_**  
(Surety for trust, Levels for SLOs, Accountability via credits)

### Key Formulas
```math
Uptime = Total Time × Availability %
Allowed Downtime = Total Time × (1 − Availability %)
SLA Violation: Actual Downtime > Allowed Downtime
Service Credit: Apply % discount based on uptime tier
```

### MCQ Tips
- **Definition**: SLA (contract) vs. SLO (metrics).
- **Calculation**: Compute allowed downtime (e.g., 1% of 720 hours = 7.2 hours).
- **Scenario**: Check violation (actual > allowed).
- **Credit**: Memorize tiers (e.g., <99.95% = 10%).

### Example MCQ
**Q**: 99% uptime, 360 hours, 4 hours downtime. Violated?  
**A**: Yes (Allowed = 3.6 hours, 4 > 3.6).

---

## 2. Cloud Economics

### Theory
- **Focus**: Cost benefits of cloud vs. owning resources.

### Cloud Properties
- **Common Infrastructure**: Shared resources (statistical multiplexing).
- **Location-Independence**: Global access, low latency.
- **Online Connectivity**: Enables access, adds network costs.
- **Utility Pricing**: Pay-per-use, ideal for variable demand.
- **On-Demand Resources**: Scalable, elastic provisioning.

### Mnemonic
**_CLOUD = Common, Location-free, Online, Utility, Demand-driven_**

### Key Formulas
```math
Demand Metrics:
  D(t): Demand over time
  P: Peak Demand = max(D(t))
  A: Average Demand = Avg(D(t))

Cost Metrics:
  B: Baseline Unit Cost (owning)
  C: Cloud Unit Cost (renting)
  U = C / B: Utility Premium

Costs:
  Baseline Cost (BT): BT = P × B × T
  Cloud Cost (CT): CT = A × U × B × T

Cloud Cheaper if: U < P/A

Penalty Cost ∝ ∫ |D(t) - R(t)| dt (where R(t) = allocated resources)
```

### Mnemonic
**_PAPA = Peak/Average Predicts Affordability_**  
(If U < P/A, cloud is cheaper)

### MCQ Tips
- **Properties**: Identify benefits (e.g., “Reduces costs?” → Common Infrastructure).
- **Costs**: Apply U < P/A, calculate BT and CT.
- **Penalty**: Recognize spiky demand = high penalty.
- **Comparison**: Cloud vs. in-house (e.g., efficiency impacts).

### Example MCQ
**Q**: P = 100, A = 50, U = 1.5. Cloud cheaper?  
**A**: Yes (P/A = 2 > 1.5)

---

## 3. MapReduce

### Theory
- **Definition**: Programming model for large-scale data processing; parallel and fault-tolerant.

### Phases
- **Map**: Splits data, produces key-value pairs (e.g., “cat” → (cat, 1)).
- **Reduce**: Aggregates pairs by key (e.g., (cat, [1, 1]) → (cat, 2)).

### Components
- Mappers
- Reducers
- Master (coordinates)

### Storage
- **HDFS** (Hadoop Distributed File System): Splits data into blocks (e.g., 64 MB).

### Mnemonic
**_MAP = Munch And Process_**  
**_REDUCE = Roll-up, End, Deliver, Unite, Count, Evaluate_**

### Key Formula
```math
HDFS Blocks = ⌈File Size / Block Size⌉
(Minimum 1 block/file)
```

### MCQ Tips
- **Phases**: Map (transform) vs. Reduce (aggregate).
- **Examples**: Word count (input → key-value → output).
- **HDFS**: Calculate blocks, watch for small files (1 block).
- **Scenario**: Identify phase outputs (e.g., Map: (dog, 1)).

### Example MCQ
**Q**: HDFS block size = 64 MB, files: 64 KB, 65 MB. Blocks?  
**A**: 3 blocks (⌈0.064/64⌉ = 1 block, ⌈65/64⌉ = 2 blocks)

---

## 4. Resource Management - I

### Theory
- **Definition**: Efficient allocation/control of cloud resources (CPU, storage, VMs) in IaaS.

### Resource Types
- **Physical**: Hardware (CPU, disk).
- **Logical**: Software (OS, APIs).

### Objectives
- Scalability
- Quality of Service (QoS)
- Cost-effectiveness
- Low latency

### Aspects
- **Provisioning**: Allocate resources to users.
- **Allocation**: Distribute economically.
- **Adaptation**: Dynamic scaling.
- **Mapping**: Match needs to resources.
- **Modeling**: Predict needs.
- **Discovery**: Find resources.
- **Scheduling**: Time resource use.

### Mnemonic
**_PRO-AMMDS = Provision, Allocate, Adapt, Map, Model, Discover, Schedule_**

### MCQ Tips
- **Definitions**: Physical vs. Logical resources.
- **Objectives**: Scalability, QoS.
- **Aspects**: Identify scenarios (e.g., “Dynamic scaling” → Adaptation).
- **Numericals**: VM provisioning:
```math
VMs = ⌈Demand / Capacity⌉
```

### Example MCQ
**Q**: What’s resource provisioning?  
**A**: Allocating provider resources to users

---

## Quick Revision Checklist

- **SLAs**: Memorize uptime formula, credit tiers.
- **Cloud Economics**: Master U < P/A, penalty concept.
- **MapReduce**: Understand phases, HDFS block calculation.
- **Resource Management**: Know aspects (PRO-AMMDS), objectives.
- **Practice**: 5–10 MCQs/day, focus on calculations.

---
