# NPTEL Cloud Computing Exam Cheatsheet

**A concise, exam-focused summary for Week 5 numericals, designed for NPTEL Cloud Computing MCQs. Ideal for rapid revision!**

---

## Table of Contents
- [1. Service Level Agreements (SLAs)](#1-service-level-agreements-slas)
- [2. Cloud Economics](#2-cloud-economics)
- [3. MapReduce (Block Calculation)](#3-mapreduce-block-calculation)
- [4. Resource Management](#4-resource-management)
- [Quick Memory Keys](#quick-memory-keys)
- [Trap Eliminations (MCQ Tips)](#trap-eliminations-mcq-tips)
- [Final MCQ Simulation (Checklist)](#final-mcq-simulation-checklist)

---

## 1. Service Level Agreements (SLAs)

### Formulas
- **Total Time** = Days × Hours/day
- **Uptime** = Total Time × SLA%
- **Allowed Downtime** = Total Time - Uptime
- **SLA Violation** = Actual downtime > Allowed downtime
- **Service Credit**:
  - <99.95% = 10%
  - <99% = 25%

### Mnemonic
*SLA = Subtract Lack, Apply Credit*

### Shortcuts
- Convert minutes to decimals (e.g., 15 mins = 0.25 hr)
- Compare downtime directly

### MCQ Trigger
If downtime > allowed → **SLA violated**

---

## 2. Cloud Economics

### Formulas
- **Baseline Cost**: \( B_T = P \times B \times T \)
- **Cloud Cost**: \( C_T = A \times U \times B \times T \)
- **Cloud Cheaper**: \( U < P/A \)
- **Penalty Cost**: Integral of |Demand - Resource|

### Mnemonic
*PAPA = Peak/Average Predicts Affordability*

### Shortcuts
- Penalty cost = Integral × per-unit cost
- Compare Utility Premium with Peak/Average ratio

### MCQ Trigger
If \( P/A > U \) → **Cloud cheaper**

---

## 3. MapReduce (Block Calculation)

### Formula
- **Blocks** = \( \lceil \text{File Size} / \text{Block Size} \rceil \)
- Minimum 1 block per file (even if tiny)

### Mnemonic
*HDFS = Huge Data, File Splits*

### Shortcuts
- Always use ceiling function
- Tiny files (KBs) = 1 block

### MCQ Trigger
If file < block → **1 block**

---

## 4. Resource Management

### Formula
- **VMs Needed** = \( \lceil \text{Demand} / \text{Capacity} \rceil \)
- **Total Cost** = VMs × Cost/VM/hr

### Shortcuts
- Simple division + ceiling

### MCQ Trigger
Demand ÷ Capacity → Ceiling → Multiply cost

---

## Quick Memory Keys

| **Topic**            | **Memory Trick**                     | **Watch for…**                       |
|-----------------------|--------------------------------------|--------------------------------------|
| SLAs                 | Subtract Lack, Apply Credit          | Compare downtime, decimals           |
| Cloud Economics      | PAPA rule                            | Compare P/A with U                   |
| MapReduce            | Ceiling rule                         | Minimum 1 block/file                 |
| Resource Management  | Simple division                      | Ceiling function for VMs             |

---

## Trap Eliminations (MCQ Tips)

- ❌ **Negative cost** = wrong option
- ❌ **Wrong units** (e.g., hours vs mins) = wrong option
- ❌ **Forgetting ceiling function** (MapReduce, VMs) = wrong

---

## Final MCQ Simulation (Checklist)

- ✅ **SLA Violation**: Compare actual downtime vs allowed
- ✅ **Cloud Cheaper**: \( P/A > U \)?
- ✅ **MapReduce**: Ceiling blocks
- ✅ **VMs and Cost**: Demand ÷ Capacity, ceiling, cost multiplication

---

### Pro Tip
Keep this cheatsheet handy for a quick glance before the exam. Focus on **ceiling functions** and **unit conversions** to ace those MCQs! 🚀
