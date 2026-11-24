# Initial Literature Analysis

## 1. Introduction

Cybersecurity in refrigeration infrastructure can be examined through research on industrial control systems (ICS), operational technology (OT), and cyber-physical systems. These systems combine digital control mechanisms with physical processes, making cybersecurity incidents potentially relevant to both system integrity and operational safety.

This initial review examines three sources that establish the technical foundation for the proposed research.

## 2. Review of Existing Literature

### 2.1 Protecting Chiller Systems from Cyberattack Using a Systems Thinking Approach

**Authors:** Shaharyar Khan and Stuart Madnick  
**Year:** 2022  
**Publication:** Network, 2(4), 606–627  
**DOI:** https://doi.org/10.3390/network2040035

**Research focus:**

The authors apply a systems-thinking approach to examine cybersecurity and safety risks in an industrial chiller plant.

**Key findings and relevance:**

- Cybersecurity weaknesses can emerge from interactions between technical components, operators, and organisational processes.
- Unauthorised changes to controller parameters can create unsafe equipment behaviour.
- Remote configuration and inadequate access restrictions can introduce security risks.
- Security analysis should consider operational consequences, not only conventional information-security concerns.

**Relevance to this research:**

This is the most directly relevant source identified so far. It establishes that industrial chiller systems deserve specific cybersecurity consideration.

**Research implication:**

The proposed research must go beyond identifying refrigeration-related cyber risks. It should investigate measurable security controls and their effectiveness under controlled experimental conditions.

### 2.2 Guide to Operational Technology (OT) Security

**Publisher:** National Institute of Standards and Technology (NIST)  
**Publication:** Special Publication 800-82, Revision 3  
**Year:** 2023  
**DOI:** https://doi.org/10.6028/NIST.SP.800-82r3

**Research focus:**

This publication provides security guidance for operational technology, including industrial control systems, programmable logic controllers, and supervisory control systems.

**Key points:**

- OT environments have distinct reliability, performance, and safety requirements.
- Security controls must account for operational constraints.
- Remote access should be justified, restricted, and monitored.
- Organisations should consider appropriate network architectures and security safeguards.

**Relevance to this research:**

This publication provides authoritative guidance for selecting and justifying network segmentation and restricted remote-access mechanisms.

**Research implication:**

The proposed framework should evaluate security improvements alongside their computational and operational overhead.

### 2.3 A Real-Time Network Based Anomaly Detection in Industrial Control Systems

**Authors:** Faeze Zare, Payam Mahmoudi-Nasr, and Rohollah Yousefpour  
**Year:** 2024  
**Journal:** International Journal of Critical Infrastructure Protection  
**Article:** 100676  
**DOI:** https://doi.org/10.1016/j.ijcip.2024.100676

**Research focus:**

The authors investigate network-based anomaly detection for industrial control systems, focusing on data manipulation attacks involving Modbus/TCP-based SCADA communication.

**Key points:**

- Network traffic can contain indicators of malicious manipulation.
- The study proposes a sequence-to-sequence anomaly detection architecture.
- The proposed approach uses LSTM-based components and attention mechanisms.

**Relevance to this research:**

The study provides a technical reference for examining abnormal network communication in an industrial control environment.

**Research implication:**

Our experiments should consider network-level anomalies and determine whether combining network observations with refrigeration process data provides additional detection value.

## 3. Preliminary Observations

The initial literature indicates three important research considerations:

1. Refrigeration and chiller systems have cybersecurity implications that extend beyond conventional IT security.
2. OT security mechanisms must account for operational reliability and safety.
3. Network-based anomaly detection is an established research direction, but its application to a specific refrigeration simulation requires careful evaluation.

## 4. Preliminary Research Gap — Not Yet Validated

The reviewed sources establish relevant foundations, but they do not yet prove that the proposed research addresses an unexplored problem.

A possible direction for further investigation is the experimental evaluation of network-level access controls together with the analysis of network traffic and refrigeration process variables in a supermarket-refrigeration-specific software testbed.

This direction must be checked against additional peer-reviewed literature before being presented as a research gap or novel contribution.

## 5. References

1. Khan, S., & Madnick, S. (2022). Protecting Chiller Systems from Cyberattack Using a Systems Thinking Approach. *Network, 2*(4), 606–627. https://doi.org/10.3390/network2040035

2. National Institute of Standards and Technology. (2023). *Guide to Operational Technology (OT) Security (NIST SP 800-82 Rev. 3).* https://doi.org/10.6028/NIST.SP.800-82r3

3. Zare, F., Mahmoudi-Nasr, P., & Yousefpour, R. (2024). A real-time network based anomaly detection in industrial control systems. *International Journal of Critical Infrastructure Protection*, Article 100676. https://doi.org/10.1016/j.ijcip.2024.100676
