# Retail Pharmacy Process Optimization & Simulation

A Business Process Management (BPM) project focused on analyzing and redesigning a high-volume retail pharmacy's customer service and dispensing workflow in Lisbon, Portugal.

The project combines BPMN 2.0 process modelling, hierarchical simulation in Bizagi, Lean process analysis, and financial feasibility assessment to identify operational bottlenecks and evaluate process redesign alternatives.

[**Read the full technical report (PDF) →**](./caring-pharmacy-bpm-report.pdf)

---

## Project Overview

The case study models a pharmacy branch handling approximately **220 customers per day**. The objective was to understand the existing process, identify sources of inefficiency, and design a more efficient workflow using process redesign and automation.

The project follows two main stages:

- **AS-IS Analysis:** Model and simulate the existing workflow to identify bottlenecks, resource utilization issues, and customer waiting times.
- **TO-BE Redesign:** Propose an optimized process using triage, parallel activities, and automation, then evaluate its expected operational and financial impact through simulation.

## Key Findings & Simulated Results

The baseline simulation identified Pharmacy Technicians as the main resource bottleneck, with a utilization rate of 73.76%.

The redesigned process was evaluated against the baseline using the same general demand context.

| Performance Metric | AS-IS | TO-BE |
|---|---:|---:|
| Average customer cycle time | 12m 00s | 5m 31s |
| Customer waiting time | ~2m 00s | <1 sec |
| Pharmacy Technician utilization | 73.76% | 12.94% |
| Pharmacist utilization | 58.87% | 53.10% |
| Estimated daily throughput capacity | ~230 | ~800+ |

**Main simulated outcomes:**
- 54% reduction in average customer cycle time.
- Customer waiting time reduced to near-zero in the simulation.
- Pharmacy Technician utilization reduced from 73.76% to 12.94%.
- Estimated throughput capacity increased from approximately 230 to over 800 customers per day.

These figures represent simulation outputs under the model's assumptions, not results from a real-world implementation.

## Process Redesign

The TO-BE model applies several BPM and Lean redesign principles:

**1. Customer Triage — Green Lane**

Introduces a fast-track route for non-prescription customers (25% of demand), allowing them to bypass unnecessary clinical checks and proceed directly to fulfillment.

**2. Parallel Activities**

Redesigns the workflow so that medication picking can take place concurrently with the pharmacist's clinical safety check.

**3. Automation**

Introduces self-service digital check-in kiosks and an Automated Dispensing System (ADS) to reduce manual workload and improve process flow.

The redesign aims to reduce unnecessary waiting, balance resource utilization, and increase the process's capacity to handle demand.

## Financial Feasibility

The proposed redesign was also evaluated from a financial perspective.

| Financial Metric | Estimated Result |
|---|---:|
| Initial investment (CAPEX) | €96,500 |
| Return on Investment (ROI) | 60.5% |
| Payback period | 1.65 years |

The financial analysis considered investment costs, operating costs, avoided labour overhead, and demand retention. A sensitivity analysis was also conducted to assess the feasibility of the proposal under different growth assumptions.

These are model-based estimates dependent on the financial assumptions documented in the technical report.

## Methodology & Tools

| Area | Methods / Tools |
|---|---|
| Process modelling | BPMN 2.0 |
| Process simulation | Bizagi Modeler & Bizagi Simulation Engine |
| Process analysis | Value-Added Analysis (VA/BVA/NVA), Lean Waste Analysis (Muda) |
| Process redesign | Triage, parallelism, automation, elimination |
| Performance evaluation | Resource utilization, cycle time, waiting time, throughput |
| Financial assessment | CAPEX/OPEX modelling, ROI, payback period, sensitivity analysis |
| Trade-off evaluation | Devil's Quadrangle |

## Repository Structure

| File | Description |
|---|---|
| [`as-is-model.bpm`](./as-is-model.bpm) | Original process model |
| [`to-be-model.bpm`](./to-be-model.bpm) | Redesigned process model |
| [`caring-pharmacy-bpm-report.pdf`](./caring-pharmacy-bpm-report.pdf) | Full 63-page technical report, including process analysis, simulation configuration, redesign rationale, financial evaluation, and sensitivity analysis |

The `.bpm` files can be opened using Bizagi Modeler.

## Project Context

Academic project developed as part of the Information Management degree at NOVA IMS.

The project demonstrates the application of Business Process Management concepts to operational process analysis, simulation-based evaluation, and process redesign in a retail pharmacy context.

## Project Documentation

- [**Full Project Report (PDF)**](./caring-pharmacy-bpm-report.pdf) — Detailed documentation of the AS-IS analysis, BPMN models, process simulation, TO-BE redesign, and financial evaluation.
- [Original Case Study & Project Brief (PDF)](./docs/project-description.pdf) — Lecturer-provided case description, business context, process requirements, and project guidelines.
