# Cloud Computing Security Cheatsheet 🚀

## Security Basics 🔐

### Core Components 🛡️
- **Confidentiality** 🤫: Hide data/resources.
- **Integrity** ✅: Untampered data (data integrity) + legit source (authenticity).
- **Availability** 🌐: Ensure access.

### Security Attacks 😈
- **Interruption** 🚫: Blocks access.
- **Interception** 🕵️‍♂️: Steals data.
- **Modification** 🖌️: Alters data (integrity attack).
- **Fabrication** 🎭: Fakes data (authenticity attack).

### Threat Classes ⚠️
- **Disclosure** 📢: Snooping.
- **Deception** 🕵️: Modification, spoofing, repudiation.
- **Disruption** 🚧: Delay, DoS.

## Policies & Mechanisms 📜
- **Policy**: Defines allowed/not allowed. 🗳️
- **Mechanisms**: Enforce policies (e.g., firewalls). 🔧
- **Conflicts**: Can create vulnerabilities. 😬

## Security Goals 🎯
- **Prevention** 🛑: Stop attacks.
- **Detection** 🔍: Catch violations.
- **Recovery** 🩹: Fix damage, keep running.

## Trust & Mechanisms 🤝
- **Policies**: Define secure states.
- **Mechanisms**: Must enforce correctly (secure, precise, broad).

## Assurance 📋
- **Specification**: Define functionality.
- **Design**: Plan system.
- **Implementation**: Build it.

## Operational Issues 💼
- **Cost-Benefit** 💸: Prevent vs. recover?
- **Risk Analysis** ⚖️: What/how much to protect?
- **Laws/Customs** 📖: Legal? Adoptable?

## Human Issues 😓
- **Organizational**: Power, financial conflicts.
- **People**: Outsiders, insiders, social engineering 🎣.

## Attacks Types 😈
- **Passive** 🦻: Eavesdropping (message contents, traffic analysis).
- **Active** 🖌️: Masquerade, replay, modification, DoS.

## Security Services 🔒
- **Confidentiality** 🤫
- **Authentication** 🕵️
- **Integrity** ✅
- **Non-repudiation** 📝
- **Access Control** 🚪
- **Availability** 🌐

## Attack Examples 😈
- Phishing 🎣
- Physical theft 🔓
- Password attacks 🔑
- Buffer overflows 💾
- Command injection 💉
- DoS 🚫
- Snooping 🕵️
- Packet manipulation 📦
- Backdoors 🚪

## Network Security Process 🌐
1. **Policy** 📜: Define usage, privacy, train users.
2. **Implement** 🛠️: Firewalls (iptables), IDS (Snort), honeypots.
3. **Recon** 🔎: Passive (undetectable) vs. active.
4. **Vuln Scanning** 🩺: Nessus, Metasploit.
5. **Pen Testing** 💥: Exploit with Metasploit or custom code.
6. **Investigation** 🕵️‍♂️: Forensics, preserve evidence.

## Firewalls & IDS 🔥
- **Firewall Types**:
  - Packet Filter: IP/port/protocol.
  - Stateful: Tracks TCP sessions.
  - Proxy: Scans all layers.
- **IDS**: Alerts on attacks.
- **Honeypot**: Decoy systems.

## Cloud Computing ☁️
- **Definition**: Scalable, on-demand, pay-as-you-go.
- **Benefits**:
  - No hardware costs 💸.
  - Dynamic scaling 📈.
  - Low startup CAPEX.
- **Challenges**:
  - Integration (50.0%).
  - Customization (49.2%).
  - Costs, regulations.

## Experiments 📊
- **Metrics**: Bandwidth, VM cost, availability, response time, cost.
- **SaaS Case Study**: 10 providers, 500 requests, QoS degradation.

## Future Scope 🔮
- Flexible QoS.
- Production workload comparison.
- Customer service classes.

**Thank You!** 🙌 Ace that exam! 😎