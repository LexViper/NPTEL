
## 📌 Cheat Sheet for Week 2

**Cloud Computing – Week 2 Cheat Sheet** 🌟  
*Quick revision for MCQs*

### ☁️ Deployment Models

- **Public Cloud** 🏬:
  - **What**: Open to all, provider-managed.
  - **Features**: Multi-tenancy (shared), mobile workloads, internet-based, elastic, low-cost, basic SLAs.
  - **Examples**: Google App Engine (PaaS), Azure (PaaS/IaaS), IBM Smart Cloud (IaaS), Amazon EC2 (IaaS).
  - **Risks**: Security (shared servers), internet outages.
- **Private Cloud** 🏡:
  - **What**: Exclusive, on-site or outsourced.
  - **On-Site**:
    - Your premises, secure, costly, limited resources.
    - Risks: Internal multi-tenancy, network limits.
  - **Outsourced**:
    - Provider-hosted, dual security, VPN links.
    - Same risks as on-site.
  - **Examples**: Eucalyptus, Ubuntu Enterprise Cloud, Amazon VPC, VMware Suite, Microsoft ECI.
- **Hybrid Cloud** 🔄:
  - **What**: Private + public mix.
  - **Features**: Secure (private), scalable (public), complex.
  - **Risks**: Insecure links, compatibility.
  - **Use Cases**: Retail surges, regulated industries.
- **Community Cloud** 🤝:
  - **What**: Shared by similar organizations.
  - **Features**: Cost-sharing, tailored security, governance challenges.
  - **Risks**: Multi-tenancy, rule disputes.
  - **Examples**: Google Cloud for Healthcare, IBM Cloud for Finance (implied).

### 🌐 Web Services

- **XML** 📝:
  - **What**: Custom tags for data exchange.
  - **Vs. HTML**: Data vs. display.
  - **Use**: Cross-platform app communication.
- **SOAP** ✉️:
  - **What**: XML messaging over HTTP.
  - **Structure**: Envelope, Header, Body, Fault.
  - **Features**: Neutral, extensible, stateless.
  - **Why**: Universal (vs. CORBA/RMI).
  - **Security**: SSL, WS-Security.
  - **Uses**: RPC, document exchange.
- **WSDL** 📖:
  - **What**: XML service contract.
  - **Parts**: Port Type, Message, Types, Binding.
  - **Purpose**: Define operations/protocols.
- **UDDI** 📋:
  - **What**: Service registry.
  - **Roles**: Registry, Provider, Requestor.
  - **Pros**: Discovery, commerce.

### 🎯 MCQ Tips

- **Deployment Models**:
  - Compare: Public (open) vs. Private (exclusive) vs. Hybrid (mixed) vs. Community (shared).
  - Examples: EC2 = Public, VPC = Private.
  - Risks: Multi-tenancy (all), governance (community).
- **Web Services**:
  - Memorize: XML (tags), SOAP (envelope), WSDL (contract), UDDI (registry).
  - SOAP vs. CORBA: Neutrality.
  - WSDL parts: Port Type, Message.
- **Practice Stems**:
  - “Public cloud risk?”
  - “Private cloud example?”
  - “SOAP’s Envelope purpose?”
  - “UDDI’s role?”

---

## 🧠 How to Nail MCQs

- **Memorize Cheat Sheet** 📋: Spend 15–20 min reviewing it 2–3 times today. Use analogies (library = public, envelope = SOAP) like Week 1’s “FRESH” mnemonic.
- **Spot Differences** 🔍:
  - Public vs. Private: Open vs. exclusive.
  - XML vs. HTML: Data vs. display.
  - SOAP vs. CORBA: Universal vs. platform-specific.
- **Write Stems** ✍️ (15 min daily):
  - “What’s multi-tenancy’s risk?”
  - “Hybrid cloud benefit?”
  - “WSDL’s role?”
  - “UDDI Service Provider?”
  - “Why SOAP for web services?”
- **Focus Areas** 🎯:
  - Examples: EC2 (Public), VPC (Private).
  - SOAP structure: Envelope, Body.
  - WSDL elements: Port Type, Binding.

