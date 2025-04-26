Got it bro!
You want the complete Week 5 guide including everything, properly structured and full — ready for revision, MCQ exam, or notes.

Here’s the full clean version combining everything you shared + completing the pending part (MapReduce + Resource Management + Summary):
I’ll keep it exam-focused, mnemonics, numericals, MCQ tips — exactly your style.

⸻

📚 Week 5 Complete Guide — NPTEL Cloud Computing (Exam-Focused)

⸻

Exam Context
	•	100-mark MCQ Exam: 12 weeks total → ~8-10 marks from Week 5 (~8-10 questions).
	•	Topics:
	•	Service Level Agreements (SLAs)
	•	Cloud Economics
	•	MapReduce
	•	Resource Management

MCQ Types:
	•	Definitions (e.g., SLA vs. SLO)
	•	Calculations (e.g., downtime %, costs, block sizes)
	•	Scenarios (e.g., MapReduce flow, cloud vs in-house)
	•	Comparisons (e.g., allocation vs provisioning)

⸻

🧠 Prep Strategy
	•	Memorize formulas and keywords with mnemonics.
	•	Practice quick calculations: %ages, ceilings, basic integrals.
	•	Focus:
	•	SLA violations
	•	Cloud cost models
	•	MapReduce phases
	•	Resource management objectives
	•	Time Management:
~1.2 min/question → skip tough ones at first.

⸻

🔥 High-Yield Topics

Topic	MCQs Expected
SLAs (Uptime, Credits)	2–3
Cloud Economics (Costs, Penalty)	2–3
MapReduce (Phases, Blocks)	2
Resource Management (Objectives, Aspects)	1–2



⸻

1. ✅ Service Level Agreements (SLAs)

Theory:
	•	SLA: Contract between Service Provider (SP) and Service Consumer (SC) guaranteeing availability & performance.
	•	SLO (Service Level Objective): Specific measurable targets (like 99.9% uptime, 5ms latency).
	•	Service Credits: Discounts or money-back in case of violations.

Purpose:
✅ Builds trust
✅ Helps select provider
✅ Ensures accountability

Mnemonic:

SLA = Surety, Levels, Accountability

⸻

Formulas:
	•	Uptime = Total time × Availability %
	•	Allowed Downtime = Total time × (1 − Availability %)
	•	SLA Violation: If actual downtime > allowed downtime → Violation
	•	Service Credit: Based on % thresholds (e.g., 10% if <99.95%, 25% if <99%)

⸻

Examples:

✅ Numerical 1
	•	Guarantee: 99% uptime, 12 hours/day, 30 days
	•	Outage: 10.75 hours
	•	Solution:
	•	Total time = 30 × 12 = 360 hours
	•	Allowed downtime = 360 × (1−0.99) = 3.6 hours
	•	Actual = 10.75 > 3.6 → SLA violated

✅ Numerical 2
	•	Guarantee: 99.95% uptime
	•	Costs: $50/day × 30 = $1500
	•	Outages total: ~9.67 hours
	•	Uptime % = (350.33 / 360) × 100 ≈ 97.31%
	•	Credit: 25% → $375 refund → Effective cost = $1125

⸻

MCQ Tips:
	•	Definition: SLA = contract, SLO = metrics
	•	Formula: Allowed downtime
	•	Scenario: Compare actual vs allowed downtime
	•	Trap: Hours/minutes conversions
	•	Shortcut: 1 min = 1/60 hr

⸻

2. ✅ Cloud Economics

Theory:
	•	Cloud focuses on cost benefits.
	•	Properties:
	•	Common Infrastructure: Resource sharing (statistical multiplexing)
	•	Location-Independence: Access anywhere
	•	Online Connectivity: Must stay connected
	•	Utility Pricing: Pay as you use
	•	On-Demand Resources: Scale up/down easily

⸻

Mnemonic:

CLOUD = Common, Location-free, Online, Utility, Demand-driven

⸻

Formulas:
	•	Demand:
	•	D(t): Demand over time
	•	P: Peak demand
	•	A: Average demand
	•	Costs:
	•	B: Baseline cost/unit
	•	C: Cloud cost/unit
	•	Utility premium: U = C/B

⸻

	•	Baseline Cost:
B_T = P × B × T
	•	Cloud Cost:
C_T = A × U × B × T
	•	Cloud Better?
If U < P/A
	•	Penalty Cost:
∝ ∫ |D(t) − R(t)| dt

⸻

Examples:

✅ Numerical 1
	•	D(t) = 50sin(t)
	•	Penalty:
~26.18 × 0.9 = 23.56 units

✅ Numerical 2
	•	P = 100, A ≈ 50.5
	•	Cloud cost cheaper if: U (1.67) < (P/A) (1.98)

✅ Numerical 3
	•	Core-hour effective costs:
	•	In-house (40% eff.): 10.6 INR/effective-hour
	•	Cloud (80% eff.): 6.72 INR/effective-hour
	•	After improving efficiency to 70%, in-house wins.

⸻

MCQ Tips:
	•	Properties: Spot words like “common”, “pay-per-use”
	•	Formulas: Apply U < P/A
	•	Penalty: If spiky demand → high penalty
	•	Trap: Units (INR/hr, core-hours)

⸻

3. ✅ MapReduce

Theory:
	•	MapReduce:
Parallel, distributed model for large-scale data (ex: Hadoop).
	•	Phases:
	1.	Map Phase:
	•	Data split into blocks
	•	(key, value) pairs generated (e.g., “dog” → (dog, 1))
	2.	Shuffle/Sort:
	•	Group keys
	3.	Reduce Phase:
	•	Combine values (e.g., (dog, [1,1]) → (dog, 2))

⸻

Mnemonic:

MAP = Munch And Process
REDUCE = Roll-up, End, Combine Usage

⸻

HDFS Storage:
	•	Data split into blocks (default 64 MB or 128 MB in Hadoop)
	•	Block replication (3 copies default) for fault tolerance.

⸻

Example (Word Count):
	•	Input: “dog cat dog”
	•	Map:
	•	(dog, 1), (cat, 1), (dog, 1)
	•	Reduce:
	•	(dog, 2), (cat, 1)

⸻

MCQ Tips:
	•	Process order: Map → Shuffle → Reduce
	•	Block size questions: 64 MB default
	•	Fault tolerance: HDFS replication (default 3x)
	•	Trap: Forgetting shuffle/sort phase.

⸻

4. ✅ Resource Management

Theory:
	•	Resource Management:
Managing resources (CPU, memory, bandwidth) in cloud to ensure efficiency.
	•	Objectives:
	•	Efficiency: Max resource use
	•	Fairness: Equitable distribution
	•	Scalability: Handle growth
	•	Elasticity: Dynamic scaling
	•	QoS: Meet service-level requirements

⸻

Aspects:
	•	Provisioning: Allocate at VM/container creation time.
	•	Scheduling: Decide when and where to run jobs.
	•	Allocation: Assign resources during runtime.
	•	Monitoring: Track usage and adjust.

⸻

Mnemonic:

P-SAM
(Provisioning, Scheduling, Allocation, Monitoring)

⸻

MCQ Tips:
	•	Provisioning = Initial setup
	•	Scheduling = Deciding time/place
	•	Allocation = Live assignment
	•	Monitoring = Dynamic adjustment
	•	Trap: Provisioning ≠ allocation (provisioning = before runtime)

⸻

📜 Final Summary Cheatsheet:

Topic	Key Focus	Mnemonic
SLAs	Downtime %, Service Credit	SLA = Surety, Levels, Accountability
Cloud Economics	U < P/A, Penalty	CLOUD, PAPA
MapReduce	Phases, Blocks, Fault Tolerance	MAP, REDUCE
Resource Mgmt	Provision vs Allocation	P-SAM



⸻

⚡ Quick 5-second MCQ Recall

If Asked	Remember
SLA Violation	Actual > Allowed Downtime
Cloud Cheaper?	U < P/A
MapReduce flow	Map → Shuffle → Reduce
Resource Actions	P-SAM



⸻

✍️ Bonus Exam Tip:
	•	If stuck: Eliminate obviously wrong options first.
	•	If confusion between 2 close options: Go for more “general” one (unless keywords match very tightly).
	•	Save hard numericals for the end.

⸻

Would you also like me to create a super quick 1-page Mind Map version for this? 🚀 (good for a 5-min revision before exam!)
Just say the word bro! 💬