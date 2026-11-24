# Literature Search Strategy and Screening Protocol

**Research Project:** A Risk-Based Cybersecurity Framework for Internet-Connected Supermarket Refrigeration Systems: Design, Implementation, and Experimental Evaluation

**Document Type:** Research Methodology – Literature Review  
**Status:** Preliminary Search Protocol  
**Research Phase:** Literature Identification and Screening

---

## 1. Introduction

A structured literature search is necessary to establish the existing state of research, identify established cybersecurity approaches, evaluate relevant technical limitations, and determine potential opportunities for further investigation.

This document defines the search methodology and screening criteria for identifying scholarly and technical literature relevant to the cybersecurity of internet-connected supermarket refrigeration systems.

Since research specifically addressing supermarket refrigeration cybersecurity may be limited, the review also considers closely related domains, including industrial control systems (ICS), operational technology (OT), heating, ventilation and air conditioning (HVAC), building management systems (BMS), industrial Internet of Things (IIoT), and cyber-physical systems (CPS).

The review will examine both established security controls and emerging detection techniques, with particular attention to their applicability to refrigeration control environments.

## 2. Research Objectives of the Literature Review

The literature review is designed to:

1. Examine documented cybersecurity threats affecting refrigeration, chiller, HVAC, and industrial control environments.
2. Evaluate existing approaches to network segmentation, access control, and secure remote connectivity.
3. Investigate network-based and process-aware anomaly detection techniques for industrial environments.
4. Examine the security implications of communication protocols used in connected industrial systems, particularly MQTT where relevant.
5. Identify methodological limitations and unresolved challenges in existing research.
6. Establish an evidence-based foundation for the proposed experimental framework.

## 3. Literature Search Sources

The following academic databases and research platforms have been selected as intended search sources.

| Database / Platform | Primary Search Purpose |
|---|---|
| IEEE Xplore | Industrial cybersecurity, ICS security, network architecture, anomaly detection |
| ACM Digital Library | Cybersecurity research, IoT security, network protection |
| ScienceDirect | Industrial control security, cyber-physical systems, detection methods |
| SpringerLink | OT security, industrial IoT, cybersecurity frameworks |
| Google Scholar | Cross-disciplinary publication discovery and citation tracking |

Additional authoritative technical material may be obtained from organisations such as NIST and relevant industrial cybersecurity research teams.

**Source classification:** Academic publications, technical standards, government guidance, and industry security reports will be classified separately. They will not be treated as equivalent forms of research evidence.

## 4. Search Strategy and Keyword Development

Search terms have been organised into thematic groups to ensure coverage of the research problem.

### 4.1 Refrigeration and Building Automation Security

- "Cybersecurity of refrigeration systems"
- "Industrial chiller cybersecurity"
- "HVAC systems" AND "cybersecurity"
- "Building management systems" AND "cyber attacks"
- "Refrigeration control systems" AND "industrial security"

### 4.2 Industrial Network Security

- "Industrial control systems" AND "network segmentation"
- "Operational technology security" AND "access control"
- "ICS network architecture" AND "cybersecurity"
- "Industrial networks" AND "remote access security"
- "Network isolation" AND "industrial control systems"

### 4.3 Anomaly Detection and Cyber-Physical Security

- "Network-based anomaly detection" AND "industrial control systems"
- "Process-aware anomaly detection" AND "ICS"
- "Cyber-physical systems" AND "intrusion detection"
- "Industrial IoT" AND "anomaly detection"
- "Control system process variables" AND "attack detection"

### 4.4 Communication Protocol Security

- "MQTT protocol" AND "security"
- "MQTT" AND "industrial IoT cybersecurity"
- "Industrial communication protocols" AND "authentication"
- "IoT messaging protocols" AND "access control"

Search strings may be refined during the review to improve relevance and identify additional terminology used by researchers.

## 5. Publication Selection Criteria

A predefined set of inclusion and exclusion criteria will be applied to maintain consistency during source screening.

### 5.1 Inclusion Criteria

A source will be considered for inclusion if it:

- Addresses cybersecurity, network protection, or anomaly detection in industrial, IoT, OT, or cyber-physical environments.
- Investigates one or more security mechanisms relevant to the research objectives.
- Provides a sufficiently documented methodology, technical analysis, experimental evaluation, or recognised security guidance.
- Has verifiable bibliographic information and an identifiable publisher or issuing organisation.
- Offers findings or technical insights applicable to connected refrigeration or comparable industrial control environments.

### 5.2 Exclusion Criteria

A source will generally be excluded if it:

- Has no meaningful relationship to the research objectives.
- Does not provide sufficient technical or methodological information for critical assessment.
- Contains unverifiable publication details.
- Is a duplicate of an already identified publication.
- Makes unsupported claims that cannot be independently evaluated.

Sources that are relevant only as background material may be retained separately without being treated as empirical research evidence.

## 6. Source Classification and Evidence Hierarchy

To avoid confusing different forms of evidence, each source will be assigned a classification.

| Source Category | Description | Intended Use |
|---|---|---|
| Peer-reviewed journal articles | Research published in scholarly journals | Primary academic evidence |
| Peer-reviewed conference papers | Research presented through recognised academic conferences | Technical methods and experimental findings |
| Technical standards and guidelines | Publications from recognised standards organisations and government bodies | Security principles and recommended controls |
| Industry security reports | Vulnerability research and technical investigations | Real-world threat context and practical security observations |
| Technical documentation | Protocol, software, and system documentation | Implementation and configuration reference |

Standards and industry reports can provide important technical context, but they will not be counted as peer-reviewed academic studies.

## 7. Literature Extraction and Critical Appraisal

Each selected publication will be examined using a consistent evidence-extraction framework.

The following information will be recorded:

| Evaluation Dimension | Information to Extract |
|---|---|
| Bibliographic information | Authors, title, year, publication venue, DOI |
| Research problem | Security problem addressed by the study |
| Research objectives | Questions or objectives investigated |
| Methodology | Analytical, experimental, simulation-based, or other approach |
| Environment | Industrial system, testbed, dataset, or simulated environment |
| Security technique | Segmentation, authentication, access control, anomaly detection, etc. |
| Evaluation metrics | Detection rate, false-positive rate, latency, performance, etc. |
| Main findings | Results and conclusions reported by the authors |
| Limitations | Constraints acknowledged by the authors or identified during critical appraisal |
| Research relevance | Relationship to supermarket refrigeration cybersecurity |

The review will distinguish between findings explicitly reported by the authors and interpretations made during this research.

## 8. Preliminary Literature Foundation

The initial investigation has identified three foundational sources:

| Source | Classification | Relevance |
|---|---|---|
| Khan and Madnick (2022), *Protecting Chiller Systems from Cyberattack Using a Systems Thinking Approach* | Peer-reviewed research | Provides refrigeration-related cybersecurity and safety context |
| NIST SP 800-82 Rev. 3 (2023), *Guide to Operational Technology (OT) Security* | Technical guidance | Provides recommendations for OT security, network architecture, and access control |
| Zare et al. (2024), *A Real-Time Network Based Anomaly Detection in Industrial Control Systems* | Peer-reviewed research | Provides a technical foundation for network-based industrial anomaly detection |

These sources establish an initial foundation but do not represent the complete literature review.

Further publications will be identified and screened before the research gap is finalised.

## 9. Research Gap Identification Approach

The research gap will be derived through comparative analysis rather than assumed in advance.

The following dimensions will be examined:

1. **Application-domain coverage:** Whether existing research directly investigates supermarket refrigeration systems or relies on related industrial environments.
2. **Network protection:** Whether existing studies evaluate segmentation and restricted communication between system components.
3. **Access security:** Whether authentication and remote-access restrictions are investigated.
4. **Detection approach:** Whether detection relies exclusively on network traffic or also considers operational process variables.
5. **Experimental evaluation:** Whether proposed techniques are evaluated using reproducible simulations, testbeds, or real industrial systems.
6. **Operational performance:** Whether security improvements are assessed alongside computational overhead and operational constraints.

The comparison will help determine whether an identifiable and feasible research opportunity exists.

No claim of originality or novelty will be made until the relevant evidence has been critically examined.

## 10. Transparency and Reproducibility

To improve the transparency of the review, the following information will be documented during the search process:

- Databases and platforms actually searched.
- Date of each search.
- Exact search queries used.
- Publication date range applied, if any.
- Number of records identified.
- Duplicate records removed.
- Records excluded during title and abstract screening.
- Full-text publications assessed.
- Final number of included sources.
- Reasons for significant exclusions.

The search process will be documented as it is performed. Search counts and screening outcomes will not be estimated or fabricated.

At this stage, the review is exploratory and structured in nature. It will not be described as a systematic literature review unless the corresponding systematic procedures have been completed and documented.

## 11. Limitations of the Search Strategy

The literature search may face several limitations:

- Research specifically addressing supermarket refrigeration cybersecurity may be limited.
- Some relevant publications may focus on broader industrial chiller, HVAC, or building automation environments.
- Access to certain full-text academic publications may be restricted.
- Different industrial environments may use different architectures and communication protocols.
- Findings from simulated environments may not directly represent the behaviour of real industrial equipment.

These limitations will be considered when interpreting the literature and defining the scope of the proposed experimental study.

## 12. Planned Next Activities

The next stage of the literature review will involve:

1. Identifying additional relevant scholarly publications.
2. Verifying publication details and source credibility.
3. Screening titles, abstracts, and available full texts.
4. Critically analysing the selected studies.
5. Updating the literature comparison matrix.
6. Identifying recurring limitations and under-investigated areas.
7. Formulating a research gap supported by the reviewed evidence.

The resulting literature review will provide the academic justification for the proposed risk-based cybersecurity framework and its experimental evaluation.

---

## References

1. Khan, M. T., & Madnick, S. (2022). *Protecting Chiller Systems from Cyberattack Using a Systems Thinking Approach*. Network, 2(4), 606–627. https://doi.org/10.3390/network2040035

2. National Institute of Standards and Technology. (2023). *Guide to Operational Technology (OT) Security* (NIST Special Publication 800-82 Rev. 3). https://doi.org/10.6028/NIST.SP.800-82r3

3. Zare, et al. (2024). *A Real-Time Network Based Anomaly Detection in Industrial Control Systems*. International Journal of Critical Infrastructure Protection, 45, Article 100676. https://doi.org/10.1016/j.ijcip.2024.100676

*Note: Verify the complete author list and bibliographic metadata against the publisher's record before submitting the final manuscript.*
