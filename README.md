# Enterprise Process Optimization & Simulation (Order-to-Cash)

A comprehensive Business Process Management (BPM) project modeling, simulating, and redesigning the Order-to-Cash (O2C) workflow of a high-volume retail pharmacy branch in Lisbon, Portugal (220 customers/day).

---

## 📌 Executive Summary
* **AS-IS Diagnosis:** A 5-stage hierarchical simulation parameterized with Poisson customer arrivals and Truncated Normal task durations revealed that Pharmacy Technicians operated as a severe system bottleneck (73.76% utilization, 12m 00s average cycle time, 17% pure queue wait time).
* **Process Redesign (TO-BE):** Applied core Lean & BPM redesign heuristics:
  * **Triage ("Green Lane"):** Fast-tracked non-prescription customers (25%) past clinical checks directly to fulfillment.
  * **Parallelism & Automation:** Integrated self-service digital check-in kiosks and an Automated Dispensing System (ADS robot) executing picking concurrently with the pharmacist's clinical safety check.
* **Operational Impact:**
  * Average customer cycle time cut by **54%** (from 12m 00s down to 5m 31s).
  * Waiting time effectively reduced to **near-zero**.
  * Technician workload slashed by **5.7x** (to 12.94%), unlocking massive surge capacity to absorb demand spikes without hiring additional staff.
* **Financial & Feasibility Justification:** Evaluated a **€96,500 CAPEX** investment against avoided labor overhead and demand retention, establishing an estimated **60.5% ROI** and a **1.65-year payback period** (profitable even under a 0% growth stress test).

---

## 📊 Key Performance Comparison

| Metric | AS-IS (Baseline) | TO-BE (Optimized) | Performance Gain |
| :--- | :---: | :---: | :---: |
| **Average Cycle Time** | 12m 00s | 5m 31s | **54% Faster** |
| **Customer Wait Time** | ~2m 00s (17%) | < 1 sec | **Eliminated** |
| **Technician Utilization** | 73.76% | 12.94% | **Load Reduced 5.7x** |
| **Pharmacist Utilization** | 58.87% | 53.10% | **Balanced & Scalable** |
| **Estimated Throughput Capacity**| ~230 orders/day | ~800+ orders/day | **Quadrupled** |

---

## 📁 Repository Structure
* `caring-pharmacy-bpm-report.pdf` — Complete 63-page technical report covering process discovery, value-added/waste analysis, issue registers, Bizagi simulation configuration, and sensitivity analysis.
* `/models` — Source `.bpm` / `.bpmn` process models for Bizagi Modeler.

---

## 🛠 Tools & Methodologies
* **Standards:** BPMN 2.0
* **Software:** Bizagi Modeler, Bizagi Simulation Engine
* **Methodologies:** Hierarchical Simulation, Lean Waste Analysis (Muda), Value-Added Analysis (VA/BVA/NVA), Redesign Heuristics (Triage, Parallelism, Automation, Elimination), Devil's Quadrangle Trade-off Evaluation, CAPEX/OPEX Financial Modeling.
