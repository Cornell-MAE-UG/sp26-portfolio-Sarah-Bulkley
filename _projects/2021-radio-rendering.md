---
layout: project
title: Spotted Lanternfly Mechanical Separator
description: A buoyancy-based mechanical agitation system that removes invasive Spotted Lanternflies from harvested grapes using density separation.
technologies: [Autodesk Fusion, 3D Printing, Mechanical Testing]
image: /assets/images/radio-machine-cad.jpg
---

<style>
/* Responsive image styling */
.responsive-image {
  max-width: 100%;
  height: auto;
  display: block;
  margin: 1.5rem 0;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.image-container {
  text-align: center;
  margin: 2rem 0;
}

.image-caption {
  font-size: 0.85rem;
  color: #666;
  text-align: center;
  margin-top: -1rem;
  margin-bottom: 1.5rem;
}

/* Table styling */
.table-wrapper {
  overflow-x: auto;
  margin: 1.5rem 0;
}

table {
  width: 100%;
  border-collapse: collapse;
  font-size: 0.9rem;
}

th, td {
  border: 1px solid #ddd;
  padding: 8px 12px;
  text-align: left;
}

th {
  background-color: #f5f5f5;
  font-weight: 600;
}

tr:nth-child(even) {
  background-color: #fafafa;
}

/* Callout / highlight boxes */
.highlight-box {
  background: #f0f7ff;
  border-left: 4px solid #2c7da0;
  padding: 1rem 1.25rem;
  margin: 1.5rem 0;
  border-radius: 0 8px 8px 0;
}

.success-box {
  background: #f0fff4;
  border-left: 4px solid #2e8b57;
  padding: 1rem 1.25rem;
  margin: 1.5rem 0;
  border-radius: 0 8px 8px 0;
}

.warning-box {
  background: #fff8f0;
  border-left: 4px solid #e67e22;
  padding: 1rem 1.25rem;
  margin: 1.5rem 0;
  border-radius: 0 8px 8px 0;
}

/* Risk table specific styling */
.risk-table th:first-child,
.risk-table td:first-child {
  font-weight: 600;
}

/* Responsive typography */
@media (max-width: 768px) {
  th, td {
    padding: 6px 8px;
    font-size: 0.8rem;
  }
  
  .highlight-box, .success-box, .warning-box {
    padding: 0.75rem 1rem;
  }
}
</style>

---

## Table of Contents
{: .no_toc}

* TOC
{:toc}

---

## Client Pitch

### Team & Stakeholders

**Team:** Pest Control  
**Clients:** Cornell CALS Extension / E&J Gallo Winery / National Grape

### The Problem

Viticulturalists in New York State are affected by the spotted lanternfly (SLF) infestation, an invasive species that contaminates the harvest. Batches are rejected from juiceries and wineries, resulting in economic loss. Traditional pest-control methods are insufficient:

- **Pesticides** come with high economic and environmental costs
- **Egg removal** proves too difficult due to the massive scale of laying locations, costing too much in labor

### Impact

Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting growing consumer demand.

### Our Solution: Centrifugal Density Separator

A high-speed rotation device that separates harvested grapes from SLF by density, removing them from the desired product.

<div class="image-container">
  <img src="/assets/images/radio-machine-cad.jpg" alt="CAD rendering of the centrifugal density separator prototype" class="responsive-image">
  <div class="image-caption">Figure 1: CAD rendering of the mechanical separator prototype</div>
</div>

**How it works:**

1. Harvest is loaded into the device
2. An internal drum spins at a calculated RPM
3. Heavier grapes are pushed out furthest, sliding down angled outer walls into a collection bin
4. Lighter insects get pulled into a secondary bag

**Why it's better than the status quo:**

| Approach | Issues |
|----------|--------|
| Pesticides | Leave taint on wine's taste profile; contaminate organic integrity |
| Manual sorting | Slow, costly, prone to human error |
| **Our solution** | Non-chemical, efficient at large scale |

### End-of-Semester Proof-of-Concept

A benchtop rotating drum prototype using grapes and 3D-printed SLF accurate to weight and size, allowing us to optimize RPM.

<div class="highlight-box">
  <strong>Success metric:</strong> Comparing the percentage of pests (SLF models) successfully sorted with the percentage of harvest lost.
</div>

### Key Risks & Unknowns

<div class="table-wrapper">
<table class="risk-table">
  <thead>
    <tr><th>Risk</th><th>Description</th><th>Mitigation</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Damage to grapes</strong></td><td>High RPM may rupture grape skins</td><td>"Burst Test" - spin grapes at incremental RPMs to identify rupture threshold</td></tr>
    <tr><td><strong>Mass variation</strong></td><td>Lanternfly soaked in juice is denser than dry one</td><td>Test with weighted 3D-printed bugs at various densities</td></tr>
    <tr><td><strong>Obstructions</strong></td><td>SLF wedged inside clusters may not separate</td><td>Test with SLF tucked inside dense clusters</td></tr>
    <tr><td><strong>Processing time</strong></td><td>Batch processing may be too slow</td><td>Measure cycle duration and compare to manual sorting speeds</td></tr>
  </tbody>
</table>
</div>

### Questions for the Client

1. How much non-grape material (stems, leaves) remains after primary harvest?
2. What is the maximum holding time between picking and crushing before quality loss?
3. Do SLF stay on the surface of clusters or retreat to the center when disturbed?
4. What reservations does this idea leave you with?

### References

- Penn State Extension. "Spotted Lanternfly." extension.psu.edu/spotted-lanternfly
- Penn State Extension. "Spotted Lanternfly Management in Vineyards." extension.psu.edu/spotted-lanternfly-management-in-vineyards
- NYS Department of Environmental Conservation. "Spotted Lanternfly." dec.ny.gov/nature/animals-fish-plants/spotted-lanternfly

---

## Functional Prototype

### Success Criteria

**Context:** Our device helps grapevine farmers mechanically separate invasive Spotted Lanternflies (SLF) from harvested grapes using water-based agitation and density-driven buoyancy.

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Criterion</th><th>Measurement</th><th>Target</th><th>Priority</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Separation Efficiency</strong></td><td>Count SLF models remaining entangled before/after 60s</td><td>≥90% separated</td><td>High</td></tr>
    <tr><td><strong>Processing Throughput</strong></td><td>Stopwatch from lid touch to ready-for-next-stage</td><td>≤4 min per 1kg batch</td><td>Medium</td></tr>
    <tr><td><strong>Operating Stability</strong></td><td>Pre/post position tracking + spillage measurement</td><td>≤2cm movement, ≤50ml loss</td><td>Medium</td></tr>
  </tbody>
</table>
</div>

### Exhibit Day Demo

We will present a 3D-printed bucket pre-filled with water and a contaminated batch of grape and SLF models. After a 30-second agitation cycle, we will:

1. Pour cleaned grapes into a transparent bowl to visually show separation
2. Weigh recovered SLF models to demonstrate Criterion 1 in real time

### Design Intent

The prototype is a **water-based agitation system** driven by a handheld drill.

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component</th><th>Material</th><th>Function</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Agitator Bucket</strong></td><td>3D-printed PLA</td><td>Stationary outer vessel holding water, grape models, and SLF models</td></tr>
    <tr><td><strong>Shaft</strong></td><td>Machined aluminum (Al 6061)</td><td>Transfers rotational motion; flange constrains vertical movement</td></tr>
    <tr><td><strong>Agitator Head</strong></td><td>3D-printed PLA</td><td>Propeller/paddle assembly creating turbulence when spun</td></tr>
    <tr><td><strong>Legs</strong></td><td>3D-printed PLA</td><td>Provides clearance for the drill to fit beneath the bucket</td></tr>
  </tbody>
</table>
</div>

### Test Models

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Model</th><th>Material</th><th>Specs</th><th>Density Target</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Grape Models</strong></td><td>3D-printed PLA</td><td>20mm diameter spheres, 4.61g</td><td>~1.1 g/cm³</td></tr>
    <tr><td><strong>SLF Models</strong></td><td>3D-printed PLA</td><td>10mm × 5mm cylinders, 1.42g</td><td>~1.0 g/cm³</td></tr>
  </tbody>
</table>
</div>

### Assembly Instructions

1. **Prepare the Shaft** – Insert aluminum shaft through bucket center hole; flange seats flush against rim
2. **Attach the Agitator Head** – Press-fit onto shaft inside bucket; should sit near bottom without contact
3. **Verify Clearance** – Rotate by hand to confirm free spinning (reference: 4.86" clearance measured)
4. **Connect the Legs** – Insert three legs into bottom holes near bucket circumference
5. **Connect the Drill** – Insert shaft tip into drill chuck; tighten securely
6. **Load the Bucket** – Fill to marked line with water, add grape and SLF models
7. **Operate** – Power drill, toggling direction every ~2 seconds for 30–60 seconds

---

## Design Tests

### Test 1: Single-Direction vs. Bi-Directional Agitation

**Goal:** Determine whether oscillating agitation improves separation efficiency.

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Metric</th><th>Single Direction</th><th>Bi-Directional</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Avg Separation</strong></td><td>79.5%</td><td>84.5%</td></tr>
    <tr><td><strong>Time to first separation</strong></td><td colspan="2">3.78s ± 0.15s</td></tr>
  </tbody>
</table>
</div>

**Outcome:** Bi-directional agitation performed marginally better with less variance.

<div class="highlight-box">
  <strong>Design Change:</strong> Need mechanical linkage or programmable motor controller to automate direction switching.
</div>

---

### Test 2: Propeller Cavitation & Turbulence Range

**Goal:** Determine if propeller creates enough "lift" to move SLF models without hitting bucket walls or grapes.

**Results:**
- Clearance from walls: **4.86 inches**
- Spillage: Low (only a few drops)
- Vortex depth increased proportionally with power

<div class="warning-box">
  <strong>Design Change:</strong> Increase propeller diameter ~2.2× original size; improve workholding diameter (3 propellers broke during testing).
</div>

---

### Test 3: Structural Integrity (Drill-to-Propeller Joint)

**Method:** 20 cycles × 30 seconds, inspecting for loosening and deformation.

**Results:**
- Cycles completed: 20 (no breakage)
- Connection play developed: **2.7 mm**
- Increased vibration/chatter in final 5 cycles

<div class="highlight-box">
  <strong>Design Change:</strong> Implement more secure mechanical lock between motor and agitator.
</div>

---

### Test 4: Leak Test

**Method:** Fill basket to highest level, count droplets over 1 minute (3 trials).

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Trial</th><th>Drops Lost</th><th>Water Loss</th></tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>11</td><td>0.55 mL</td></tr>
    <tr><td>2</td><td>7</td><td>0.35 mL</td></tr>
    <tr><td>3</td><td>14</td><td>0.70 mL</td></tr>
  </tbody>
</table>
</div>

**Outcome:** TPU shaft seal performs well, but tolerances need improvement.

<div class="highlight-box">
  <strong>Design Change:</strong> Source actual shaft seal from McMaster-Carr for watertight operation.
</div>

---

## Client Report

**Team Name:** F4 Pest Control  
**Team Members:** Liz Tipton, Katelyn Fu, Arda Griffin, Sarah Bulkley, Junseok Kang  
**Date:** May 5, 2026

### Context and Problem Statement

Invasive Spotted Lanternflies pose a significant **$8.8 million threat** to the regional grape population [1]. National food regulations mandate SLF removal before final production. Currently, entire batches are often discarded if contamination is found.

Our team focused on a **post-harvest solution** leveraging physical density differences between insects and fruit.

<div class="highlight-box">
  <strong>Primary constraint:</strong> Achieve ≥90% separation efficiency to meet industrial standards.
</div>

### Final Prototype

A water-based mechanical agitation system. Contaminated grapes are placed in the basin and agitated with a propeller — SLF rise to the surface, grapes sink due to density differences.

<div class="success-box">
  <strong>Result:</strong> 93% separation efficiency (exceeding 90% goal)
</div>

### Testing Results

#### Test 1: Identifying Optimal RPM

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>RPM Range</th><th>Observation</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>~3000 RPM</strong></td><td>Peak separation (93% efficiency)</td></tr>
    <tr><td>Below 3000</td><td>Grape models sink, SLF separate effectively</td></tr>
    <tr><td>Above 4000</td><td>Grapes float with SLF due to excessive vortex</td></tr>
  </tbody>
</table>
</div>

#### Test 2: Leak Test Results

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Leak-Prone Area</th><th>Drops per Minute</th></tr>
  </thead>
  <tbody>
    <tr><td>Area 1 (side wall interface)</td><td>0</td></tr>
    <tr><td>Area 2 (side wall interface)</td><td>0</td></tr>
    <tr><td>Area 3 (side wall interface)</td><td>0</td></tr>
    <tr><td>Agitator (shaft/bearing)</td><td>15</td></tr>
  </tbody>
</table>
</div>

**Finding:** Sealant/glue sufficient for side walls. Shaft/bearing interface requires redesign.

### Conclusions & Recommendations

**Success:** 93.3% separation efficiency exceeds 90% target.

**For industrial scaling:**

- Manufacture side walls as single unit to eliminate seam leaks
- Use motor capable of constant 3,000 RPM under load
- Transition to non-corrosive materials (food-safe plastics/metals)
- Address food safety: RTV sealant and PETG are food-safe, but lubricant and glue are not

**Limitations:**

- Most components custom → higher per-unit cost
- No SLF extraction mechanism for continuous operation
- Grape juice diluted with water — harvest loss potential

---

## Bill of Materials

### 3D-Printed Components

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component</th><th>Description</th><th>Quantity</th><th>Cost (USD)</th></tr>
  </thead>
  <tbody>
    <tr><td>Side Walls</td><td>Three pieces connecting to baseplate</td><td>3</td><td>$25.36</td></tr>
    <tr><td>Agitator</td><td>Propeller and shaft fitting into motor</td><td>1</td><td>$2.84</td></tr>
    <tr><td>Baseplate</td><td>Houses bearing and o-ring for leak prevention</td><td>1</td><td>$12.85</td></tr>
    <tr><td>Stand</td><td>Houses motor and speed controller</td><td>1</td><td>$35.25</td></tr>
  </tbody>
</table>
</div>

### Off-the-Shelf Components

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component</th><th>Description</th><th>Quantity</th><th>Cost (USD)</th></tr>
  </thead>
  <tbody>
    <tr><td>Ball Bearing</td><td>Reduces friction for agitator</td><td>1</td><td>$28.17</td></tr>
    <tr><td>Spring-loaded O-ring</td><td>Reduces leakage around shaft</td><td>1</td><td>$4.98</td></tr>
    <tr><td>Motor</td><td>High torque DC 12/24V, 3500/7000 RPM</td><td>1</td><td>$22.99</td></tr>
    <tr><td>Speed Controller</td><td>PWM DC motor controller</td><td>1</td><td>$12.73</td></tr>
    <tr><td>Power Supply</td><td>24V 3A 72W with on/off switch</td><td>1</td><td>$13.85</td></tr>
    <tr><td>Sealing Hex Head Screw</td><td>1/4-20, connects side walls to baseplate</td><td>6</td><td>$15.06</td></tr>
    <tr><td>1/4-20 Nut</td><td>Used with bolts</td><td>6</td><td>$0.76</td></tr>
    <tr><td>1/4-20 Heat Insert</td><td>Fused into stand for connections</td><td>6</td><td>$2.40</td></tr>
    <tr><td>RTV Sealant</td><td>Aluminum color, vibration-resistant waterproofing</td><td>1</td><td>$12.89</td></tr>
  </tbody>
</table>
</div>

**Total:** ~$177.00

---

## References

1. Cornell University News. "Spotted Lanternflies Could Cost NYS Grape Industry Millions." Jan 2025.

2. United States Department of Agriculture. "United States Standards for Grades of Grapes for Processing and Freezing." Sept 1977. Reprinted Jan 1997.

3. Zuritz, C. et al. (2005). "Density, viscosity and coefficient of thermal expansion of clear grape juice." *Journal of Food Engineering*, 71, 143-149.

4. Kühsel, S. et al. (2016). "Surface area - volume ratios in insects." *Insect Science*, 24.