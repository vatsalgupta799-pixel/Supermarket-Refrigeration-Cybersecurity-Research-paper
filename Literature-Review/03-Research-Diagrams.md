# Research Diagrams and Conceptual Models

**Project:** Cybersecurity of Internet-Connected Supermarket Refrigeration Systems

**Document Type:** Research Architecture and Methodology Visualisation

**Status:** Preliminary Research Design

---

## 1. Literature Synthesis and Research Foundation

The following conceptual diagram illustrates how the three foundational publications inform different aspects of the proposed research.

```mermaid
flowchart TD
    A["Existing Cybersecurity Literature"]

    A --> B["Khan and Madnick (2022)"]
    A --> C["NIST SP 800-82 Rev. 3 (2023)"]
    A --> D["Zare et al. (2024)"]

    B --> E["Refrigeration and Chiller<br/>Cybersecurity Risks"]
    C --> F["OT Security Controls<br/>and Architecture"]
    D --> G["Industrial Network<br/>Anomaly Detection"]

    E --> H["Research Foundation"]
    F --> H
    G --> H

    H --> I["Proposed Research Direction"]

    I --> J["Network-Level Protection"]
    I --> K["Process-Aware<br/>Anomaly Detection"]

    J --> L["Experimental Evaluation"]
    K --> L
```

**Interpretation**

The literature establishes three complementary foundations:

- Refrigeration-specific cybersecurity risks.
- Security architecture and protective controls for OT environments.
- Anomaly detection in industrial network communications.

The proposed study investigates their application within a controlled supermarket refrigeration simulation. This diagram represents the conceptual relationship between the literature and the research direction; it does not imply that the existing publications proposed the combined framework.

---

## 2. Proposed Cybersecurity Framework Architecture

This diagram illustrates the planned software-based experimental architecture.

```mermaid
flowchart TB
    subgraph PROCESS["1. Simulated Refrigeration Environment"]
        S["Temperature Sensor Simulator"]
        C["Refrigeration Controller"]
        P["Setpoints and Operating States"]
        S --> C
        C <--> P
    end

    subgraph COMM["2. Communication Layer"]
        M["MQTT Broker"]
        T["Simulated Control and Telemetry Messages"]
        M <--> T
    end

    subgraph PROTECTION["3. Security Enforcement Layer"]
        N["Network Segmentation"]
        A["Restricted Access Control"]
        N --> A
    end

    subgraph MONITOR["4. Security Monitoring Layer"]
        NT["Network Traffic Analysis"]
        PT["Process-Variable Analysis"]
        AD["Anomaly Detection Engine"]
        NT --> AD
        PT --> AD
    end

    subgraph OUTPUT["5. Evaluation and Reporting"]
        AL["Security Alerts"]
        LOG["Event and Experiment Logs"]
        MET["Performance Metrics"]
        AL --> LOG
        LOG --> MET
    end

    PROCESS <--> COMM
    COMM <--> PROTECTION
    COMM --> MONITOR
    PROTECTION --> MONITOR
    MONITOR --> OUTPUT
```

**Architecture description**

The proposed architecture consists of five logical layers:

**Layer 1 — Simulated Refrigeration Environment**

Generates temperature readings, setpoints, equipment states, and simulated control activities.

**Layer 2 — Communication Layer**

Represents communication between the simulated refrigeration components using MQTT, subject to final implementation decisions.

**Layer 3 — Security Enforcement Layer**

Implements network-level isolation and restricted access to reduce unauthorised communication and control activities.

**Layer 4 — Security Monitoring Layer**

Analyses network events and refrigeration process variables to identify suspicious behaviour.

**Layer 5 — Evaluation and Reporting Layer**

Records security events, detection outcomes, and performance measurements for comparative analysis.

**Design note:** This is a proposed architecture, not an implemented system. Exact component placement, traffic paths, and enforcement mechanisms will be finalised during testbed design.

---

## 3. Experimental Research Methodology

The experimental workflow will compare three security configurations under consistent normal and simulated adversarial conditions.

```mermaid
flowchart TD
    A["Research Questions and Hypotheses"]
    B["Design Experimental Testbed"]
    C["Generate Normal Refrigeration Behaviour"]
    D["Define Simulated Attack Scenarios"]
    E["Prepare Experimental Dataset"]

    A --> B
    B --> C
    B --> D
    C --> E
    D --> E

    E --> F["Baseline Configuration"]
    E --> G["Configuration A:<br/>Segmentation and Access Control"]
    E --> H["Configuration B:<br/>Configuration A + Anomaly Detection"]

    F --> I["Collect Experimental Results"]
    G --> I
    H --> I

    I --> J["Calculate Evaluation Metrics"]
    J --> K["Comparative Statistical Analysis"]
    K --> L["Evaluate Research Hypotheses"]
    L --> M["Document Findings and Limitations"]
```

**Experimental workflow**

1. Develop a controlled software-based refrigeration simulation.
2. Define normal operating conditions and simulated adversarial events.
3. Prepare labelled experimental scenarios.
4. Execute the scenarios under all three security configurations.
5. Collect logs, detection outcomes, and resource measurements.
6. Calculate evaluation metrics.
7. Compare results and assess the research hypotheses.
8. Document findings, limitations, and reproducibility details.

---

## 4. Comparative Security Configuration

| Configuration | Network Segmentation | Restricted Access | Anomaly Detection |
|---|---|---|---|
| Baseline | No additional segmentation | No additional access restrictions | Disabled |
| Configuration A | Enabled | Enabled | Disabled |
| Configuration B | Enabled | Enabled | Enabled |

The baseline represents the experimental reference condition, not a recommendation to operate real refrigeration equipment without security controls.

---

## 5. Experimental Evaluation Metrics

```mermaid
flowchart TD
    A["Experimental Data"]

    A --> B["Security Effectiveness"]
    A --> C["Detection Performance"]
    A --> D["Operational Overhead"]

    B --> E["Attack Success Rate"]
    C --> F["Precision and Recall"]
    C --> G["False-Positive Rate"]
    C --> H["Detection Latency"]
    D --> I["CPU Utilisation"]
    D --> J["Memory Consumption"]

    E --> K["Comparative Evaluation"]
    F --> K
    G --> K
    H --> K
    I --> K
    J --> K

    K --> L["Security-Performance Assessment"]
```

The evaluation will examine both preventive and detective security capabilities. Results will be derived from executed experiments rather than estimated or assumed values.

---

## 6. Research Design Status

| Component | Current status |
|---|---|
| Literature foundation | Initial review completed |
| Conceptual research direction | Preliminary |
| Security architecture | Proposed |
| Experimental workflow | Planned |
| Simulation implementation | Not started |
| Experimental validation | Pending |
| Quantitative results | Pending |

**Research integrity statement:** All diagrams represent proposed research concepts and planned experimental procedures. They should not be interpreted as evidence of an implemented or experimentally validated system.
