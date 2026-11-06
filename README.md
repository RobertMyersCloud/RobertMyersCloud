# Robert J. Myers

Navy veteran moving into **security operations and incident response**, with digital forensics as the long-term direction.

I spent 20 years in the Navy, most of it in supply, finance, and logistics, including about three years running a command IT department and five years as Command Security Manager. A lot of that work was investigative: tracing transactions through supply-system records to find money that had gone missing, working fraud, waste, and abuse cases, and handling security investigations and insider-threat reporting. I'm now building the technical side of that work in my own lab, and every project here is backed by evidence I collected myself.

---

## Selected Work

### [PCAP Pattern Detector](https://github.com/RobertMyersCloud/pcap-pattern-detector): scan and beacon detection in Python

Two detectors that read a packet capture and flag port scanning and beacon-like traffic. I tested them on new traffic from my lab, including traffic built to get past them. That testing found two bugs: a fast scan hidden by one later connection, and retried SYNs counted as new connections. I fixed both, set the beacon threshold from measurements, and listed the limits that remain.

### [Prove-It](https://github.com/RobertMyersCloud/prove-it) — network foundations

You can't spot abnormal traffic until you know what normal looks like. This repository is where I prove I know normal, from Ethernet and ARP up through routing, NAT, VLANs, and access control, all on a segmented lab range I built and tested.

- An isolated lab range behind a router trust boundary, with the egress policy tested
- Packet-level analysis of ARP, TCP/UDP, DNS, and HTTP/TLS
- Routing and path selection, including a test that showed my hypervisor was forwarding traffic it shouldn't, and the fix
- VLAN segmentation with inter-VLAN ACLs, verified on the wire
- A protected enclave with layered router and host firewall controls. A re-test found five gaps in my own design, and I documented each fix

Each project is one documented run. When a later test proves something wrong, the finding and the fix go into the same project.

### [Packet Analysis Lab](https://github.com/RobertMyersCloud/packet-analysis-lab) — traffic investigation

tcpdump and Wireshark analysis of normal traffic, failed connections, and controlled suspicious patterns: port enumeration and periodic beacon-like traffic. The focus is on what the packets actually support and where the evidence stops.

---

## How I Work

**Build -> Test -> Find what's wrong -> Fix -> Re-test -> Write it down**

Claims are limited to what the evidence shows. Raw captures and anything identifying stay off GitHub; screenshots are sanitized before they're published.

---

## Certifications

- GIAC Foundational Cybersecurity Technologies (GFACT)
- CompTIA Security+
- CompTIA Network+
- ISC2 Certified in Cybersecurity (CC)
- Fortinet FortiGate 7.6 Operator, Fortinet Certified Associate Cybersecurity
- AWS Certified Cloud Practitioner, Microsoft AZ-900, Microsoft SC-900
- CSA CCSK v5, CSA CCZT

**In progress:** GIAC Security Essentials (GSEC) through SANS SEC401

---

## Background

**U.S. Navy, 2001-2021**
- Command Security Manager: access and clearance actions, security investigations, insider-threat reporting
- Command IT department lead: Active Directory permissions, account provisioning, CAC/PKI
- Supply and finance: traced transactions through supply-system records to recover funds and support fraud, waste, and abuse cases
- Led teams of up to 78 people and held accountability for more than 25,000 assets

**After the Navy:** Federal Bureau of Prisons, then supply-chain management in aerospace production, where part of the job was vetting suppliers and catching false certification claims.

---

## Education

- **SANS Technology Institute** — B.S. Applied Cybersecurity, Cyber Defense (in progress)
- **University of the Incarnate Word** — MBA
- **Colorado Technical University** — B.S. Accounting

---

[LinkedIn](https://linkedin.com/in/robertjmyers5)
