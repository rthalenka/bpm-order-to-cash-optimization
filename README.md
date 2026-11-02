# Pharmacy Process Optimization | BPMN & Bizagi Simulation

An end-to-end Business Process Management (BPM) project focused on analyzing and redesigning the customer service and dispensing workflow of a high-volume retail pharmacy branch.

Using BPMN 2.0 modeling, hierarchical process simulation and Lean process improvement principles, the project identifies operational bottlenecks, evaluates redesign alternatives and assesses their financial feasibility.

## Project Overview

The project examines the operational workflow of a retail pharmacy serving approximately 220 customers per day.

The initial process was analyzed to identify bottlenecks, waiting times and resource utilization issues. Based on these findings, a redesigned process was developed to improve customer flow, reduce unnecessary waiting and increase operational capacity.

The analysis covers two process scenarios:

- **AS-IS:** Modeling and simulation of the existing operational workflow.
- **TO-BE:** Redesign and simulation of an optimized workflow incorporating process automation, task parallelization and customer segmentation.

## Key Results

The Bizagi simulation produced the following comparison between the baseline and redesigned scenarios:

| Performance Metric | AS-IS | TO-BE |
|---|---:|---:|
| Average customer cycle time | 12m 00s | 5m 31s |
| Customer waiting time | ~2m 00s | Less than 1 second |
| Technician utilization | 73.76% | 12.94% |
| Pharmacist utilization | 58.87% | 53.10% |
| Estimated daily throughput capacity | ~230 orders | ~800+ orders |

**Main outcomes:**

- 54% reduction in average customer cycle time.
- Waiting time reduced to near-zero in the simulated scenario.
- Technician utilization reduced by approximately 5.7 times.
- Increased estimated throughput capacity, creating additional operational capacity to accommodate demand fluctuations.

## Process Redesign

The TO-BE model introduces several process improvement measures:

**1. Customer Segmentation and Triage**

A dedicated fast-track route ("Green Lane") was introduced for non-prescription customers, representing approximately 25% of demand. These customers bypass unnecessary clinical checks and proceed directly to fulfillment.

**2. Task Parallelization**

The dispensing process was redesigned to allow medication picking to occur concurrently with the pharmacist's clinical safety check, reducing sequential processing time.

**3. Process Automation**

The proposed workflow integrates:

- Digital self-service check-in kiosks.
- An Automated Dispensing System (ADS) to support medication picking.
- Improved coordination between pharmacy technicians and pharmacists.

These changes aim to reduce manual workload, eliminate unnecessary process steps and improve resource allocation.

## Financial Feasibility

The redesigned process was also evaluated from a financial perspective to assess whether the proposed operational improvements could justify the required investment.

| Financial Metric | Estimated Result |
|---|---:|
| Initial investment (CAPEX) | €96,500 |
| Estimated ROI | 60.5% |
| Estimated payback period | 1.65 years |

The financial analysis also included sensitivity testing, including a 0% growth scenario, to assess the investment's feasibility under more conservative assumptions.

*Financial results are estimates based on the project's modeling assumptions and should not be interpreted as realized business performance.*

## Methodology

The project follows a structured BPM lifecycle:

1. **Process Discovery and Modeling:** Documentation of the existing workflow using BPMN 2.0.
2. **AS-IS Analysis:** Identification of bottlenecks, process inefficiencies and non-value-added activities.
3. **Simulation:** Development of a hierarchical Bizagi simulation using Poisson customer arrivals and truncated normal task-duration distributions.
4. **Process Redesign:** Application of Lean principles and redesign heuristics, including triage, parallelization, automation and process elimination.
5. **TO-BE Simulation:** Evaluation of the redesigned workflow and comparison against baseline performance.
6. **Financial Evaluation:** CAPEX/OPEX analysis, ROI estimation, payback period calculation and sensitivity analysis.

## Tools & Methodologies

| Category | Tools / Concepts |
|---|---|
| Process modeling | BPMN 2.0 |
| Simulation | Bizagi Modeler, Bizagi Simulation Engine |
| Process improvement | Lean Management, Muda Analysis |
| Process analysis | Value-Added Analysis (VA/BVA/NVA) |
| Redesign techniques | Triage, Parallelism, Automation, Elimination |
| Performance evaluation | Devil's Quadrangle |
| Financial analysis | CAPEX/OPEX, ROI, Payback Period, Sensitivity Analysis |

## Repository Structure

```text
bpm-order-to-cash-optimization/
│
├── as-is-model.bpm
├── to-be-model.bpm
├── caring-pharmacy-bpm-report.pdf
└── README.md
```

- `as-is-model.bpm` – Bizagi source model representing the existing process.
- `to-be-model.bpm` – Bizagi source model representing the redesigned workflow.
- `caring-pharmacy-bpm-report.pdf` – Complete technical report covering process discovery, waste analysis, simulation configuration, redesign decisions and financial evaluation.

## Project Context

Academic project developed as part of the Information Management degree at NOVA IMS.

The project demonstrates the application of Business Process Management principles to a practical operational challenge, combining process modeling, simulation, performance analysis and business-oriented decision-making.
