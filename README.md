# Project 1: Cybersecurity of Internet-Connected Supermarket Refrigeration Systems

## Research Title

**A Risk-Based Cybersecurity Framework for Internet-Connected Supermarket Refrigeration Systems: Design, Implementation, and Experimental Evaluation**

---

## 1. Abstract and Research Overview

The increasing adoption of Internet of Things (IoT) technologies and remote-management capabilities in commercial refrigeration infrastructure has introduced new cybersecurity challenges for supermarket environments. Modern refrigeration systems rely on network-connected controllers, temperature sensors, monitoring platforms, and remote-access interfaces to maintain equipment functionality and preserve temperature-sensitive products.

Although connectivity improves operational visibility and management efficiency, it also expands the potential attack surface. Security weaknesses may expose refrigeration control infrastructure to unauthorized access, manipulation of operational parameters, malicious command execution, and disruption of critical refrigeration processes.

This research proposes the design and experimental evaluation of a risk-based cybersecurity framework for internet-connected supermarket refrigeration systems. The proposed framework will investigate three complementary security mechanisms: network segmentation, restricted remote access, and process-aware anomaly detection. A controlled, software-based experimental environment will be developed to evaluate their effectiveness under simulated normal and adversarial operating conditions.

The evaluation will consider security effectiveness alongside operational performance, including detection accuracy, false-positive rates, detection latency, and computational overhead. The study aims to provide a reproducible experimental assessment of cybersecurity controls relevant to connected refrigeration environments.

## 2. Research Problem and Motivation

Supermarket refrigeration systems increasingly operate within interconnected digital environments involving operational technology (OT), IoT devices, industrial controllers, and remote-management infrastructure.

The integration of these technologies creates potential pathways for cyber threats that may affect both information security and physical operations. Unauthorized modifications to temperature setpoints, malicious control commands, and unexpected network communications could compromise system integrity and operational availability.

Traditional network security mechanisms provide important protective capabilities; however, their effectiveness and operational trade-offs must be examined in the context of refrigeration-specific control activities.

**Central Research Problem:**

How can a risk-based cybersecurity framework combining network-level protection and process-aware anomaly detection reduce unauthorized access and suspicious control activities in internet-connected supermarket refrigeration systems while maintaining acceptable operational performance?

## 3. Research Aim and Objectives

### 3.1 Research Aim

To design and experimentally evaluate a risk-based cybersecurity framework that strengthens the protection of internet-connected supermarket refrigeration control systems through network security and process-aware anomaly detection.

### 3.2 Research Objectives

1. **Threat Identification:** Examine cybersecurity threats, vulnerabilities, and attack surfaces associated with connected refrigeration control environments.
2. **Security Architecture:** Develop a security framework incorporating network segmentation, restricted remote access, and anomaly monitoring.
3. **Access-Control Evaluation:** Assess the effectiveness of network-level security controls in preventing unauthorized communication and control activities.
4. **Anomaly Detection:** Investigate the detection of suspicious behaviour through the analysis of network traffic and simulated refrigeration process data.
5. **Performance Assessment:** Quantitatively evaluate detection effectiveness, false alarms, response latency, and computational overhead.
6. **Comparative Analysis:** Compare baseline and security-enhanced configurations to identify the effectiveness and limitations of the proposed mechanisms.

## 4. Research Questions

The study will investigate the following research questions:

- **RQ1:** What are the principal cybersecurity threats and vulnerabilities associated with internet-connected supermarket refrigeration control systems?
- **RQ2:** To what extent can network segmentation and access-control mechanisms mitigate unauthorized communication and control activities?
- **RQ3:** Can the combined analysis of network traffic and refrigeration process variables improve the identification of suspicious operational behaviour?
- **RQ4:** What security-performance trade-offs emerge when network-level protection and process-aware anomaly detection are implemented together?

## 5. Proposed Research Methodology

### 5.1 Research Approach

The study will adopt a quantitative, experimental research approach using a controlled software-based testbed. The testbed will simulate essential refrigeration control operations and generate representative network and process-level events.

This approach will allow repeatable experimentation without requiring access to commercial refrigeration equipment or live supermarket infrastructure.

### 5.2 Experimental Environment

A simulated refrigeration controller will be developed to represent selected operational characteristics of a commercial refrigeration system.

The simulation will generate:

- Temperature measurements and operating thresholds.
- Configurable temperature setpoints.
- Refrigeration equipment states.
- Control commands and system events.
- Simulated network communication.
- Normal and abnormal operational scenarios.

The generated data will provide the basis for evaluating security controls and anomaly-detection mechanisms.

### 5.3 Security Configurations

The proposed framework will be evaluated using three experimental configurations:

| Configuration | Description |
|---|---|
| Baseline | Simulated refrigeration environment without the additional security mechanisms under evaluation. |
| Configuration A | Network segmentation and restricted remote-access controls. |
| Configuration B | Configuration A enhanced with process-aware and network-based anomaly detection. |

A consistent set of normal and simulated adversarial scenarios will be applied across the configurations to support comparative analysis.

### 5.4 Simulated Security Scenarios

The experimental evaluation will consider scenarios such as:

- Unauthorized attempts to connect to refrigeration control services.
- Unauthorized modification of temperature setpoints.
- Unexpected or suspicious control commands.
- Abnormal temperature measurements and operating states.
- Unexpected network communication patterns.

All experiments will be conducted exclusively within the isolated research testbed.

## 6. Performance Evaluation and Research Metrics

The effectiveness of the proposed framework will be evaluated using the following metrics:

| Metric | Purpose |
|---|---|
| Attack Success Rate | Measures the proportion of simulated attacks that successfully achieve their intended objective. |
| Detection Rate (Recall) | Measures the proportion of actual simulated malicious events correctly detected. |
| Precision | Measures the proportion of detected events that are genuinely malicious within the labelled test dataset. |
| False-Positive Rate | Measures the proportion of normal events incorrectly classified as malicious. |
| Detection Latency | Measures the time required to identify a simulated malicious event. |
| CPU Utilisation | Evaluates the computational processing overhead introduced by the security mechanisms. |
| Memory Consumption | Measures additional memory requirements during experimental execution. |

The results will be analysed comparatively across the three configurations. Any performance claims will be based on measured experimental data.

## 7. Proposed Technology Stack

The following technologies are under consideration for developing the experimental environment:

| Technology | Intended Application |
|---|---|
| Python | Simulation development, security logic, and experimental automation. |
| MQTT / Mosquitto | Simulated IoT communication and message exchange. |
| Wireshark | Network traffic inspection and protocol analysis. |
| Pandas | Experimental dataset processing and statistical analysis. |
| Matplotlib | Visualisation of experimental results. |
| Docker / Linux Network Namespaces | Isolation and network-level experimental configurations, subject to feasibility. |

The final technology stack will be selected based on implementation feasibility, experimental requirements, and reproducibility.

## 8. Expected Research Contributions

The research will investigate the following potential contributions:

1. A structured threat assessment of internet-connected supermarket refrigeration control environments.
2. A reproducible software-based experimental testbed representing selected refrigeration operations and security scenarios.
3. A comparative evaluation of network segmentation, restricted remote access, and process-aware anomaly detection.
4. An empirical assessment of security effectiveness and computational overhead.
5. Identification of implementation limitations and opportunities for future research.

These contributions will be refined following the literature review and validation of the research gap.

## 9. Research Scope and Limitations

The research is limited to a controlled, software-based simulation of selected refrigeration control and communication behaviours.

The study will not involve physical refrigeration hardware, live supermarket infrastructure, or testing against production industrial control systems.

Consequently, the findings will represent the behaviour of the implemented experimental model rather than a direct validation of security effectiveness across all commercial refrigeration installations.

The limitations of synthetic data, simulated attack scenarios, and the absence of physical process dynamics will be explicitly considered when interpreting the results.

## 10. Research Integrity and Reproducibility

The research will follow the following principles:

- All experiments will be conducted in an isolated and controlled environment.
- No production systems or third-party infrastructure will be targeted.
- Experimental results will be generated through actual test execution and will not be fabricated.
- Academic publications, technical standards, and security advisories will be cited appropriately.
- Research gaps and novelty claims will be established through critical literature analysis.
- Experimental procedures, configurations, and relevant code will be documented to support reproducibility.
- Methodological limitations and potential sources of bias will be reported transparently.

## 11. Project Status and Research Milestones

**Current Status:** Research planning and problem formulation.

**Immediate Milestone:** Conduct a structured literature review of refrigeration-system cybersecurity, industrial control system security, network segmentation, and process-aware anomaly detection.

**Subsequent Milestones:**

1. Identify and validate the research gap.
2. Finalise research questions and experimental hypotheses.
3. Design the software-based experimental testbed.
4. Implement the proposed security configurations.
5. Execute controlled experiments and collect results.
6. Analyse findings and evaluate research hypotheses.
7. Prepare the research manuscript and supporting documentation.

---

**Research Area:** Cybersecurity | Industrial Control Systems (ICS) | Operational Technology (OT) | Internet of Things (IoT) Security

**Research Type:** Experimental and Quantitative

**Experimental Environment:** Isolated Software-Based Simulation
