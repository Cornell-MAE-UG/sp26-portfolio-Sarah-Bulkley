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
- **Egg removal** proves too difficult because of the massive scale of laying locations, costing too much in labor

### Impact

Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting growing consumer demand.

### Solution: Centrifugal Density Separator

A high-speed rotation device that separates harvested grapes from SLF by density, removing them from the desired product.

<div class="image-container">
  <img src="/assets/images/radio-machine-cad.jpg" alt="CAD rendering of the centrifugal density separator prototype" class="responsive-image">
  <div class="image-caption">Figure 1: CAD rendering of the mechanical separator prototype</div>
</div>

**How to implement:**
1. Harvest is loaded into the device
2. An internal drum spins at a calculated RPM
3. Heavier grapes are pushed out furthest, sliding down angled outer walls into a collection bin
4. Lighter insects get pulled into a secondary bag

**Why it's better than the status quo:**
- Pesticides leave a taint on the wine's taste profile and contaminate the organic integrity of the grapes
- Manual sorting is slow, costly, and prone to human error/inconsistencies
- Our solution is non-chemical and efficient on a large scale

### End-of-Semester Proof-of-Concept

A benchtop rotating drum prototype using grapes and 3D-printed SLF accurate to weight and size, allowing us to optimize RPM.

<div class="highlight-box">
  <strong>Success metric:</strong> Success is determined by comparing the percentage of pests (SLF models) successfully sorted with the percentage of harvest lost.
</div>

### Key Risks & Unknowns

<div class="table-wrapper">
<table class="risk-table">
  <thead>
    <tr><th>Risk</th><th>Description</th><th>Mitigation</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Damage to grapes</strong></td><td>A high RPM exerts a force on the grape skin, possibly causing the grapes to break apart</td><td>Physical "Burst Test" - spinning grapes at incremental RPMs to identify when skins rupture</td></tr>
    <tr><td><strong>Mass variation</strong></td><td>A lanternfly soaked in grape juice is much denser than a dry one</td><td>Test with weighted 3D-printed bugs at various densities</td></tr>
    <tr><td><strong>Obstructions</strong></td><td>An SLF wedged inside a tight cluster might not separate easily</td><td>Test with SLF tucked inside dense clusters or higher-density SLF models</td></tr>
    <tr><td><strong>Processing time</strong></td><td>A centrifuge is often a batch process; if too slow, farmers will reject it</td><td>Test cycle duration and calculate throughput compared to manual sorting speeds</td></tr>
  </tbody>
</table>
</div>

### Questions for the Client

1. How much material other than grapes, like stems and leaves, typically remains in the bin after your primary harvest?
2. What is the maximum holding time allowed between the grape being picked and it reaching the crusher before you worry about quality loss?
3. Do the SLF tend to stay on the surface of the grape clusters when disturbed, or do they retreat deep into the center of the bunch?
4. What reservations does this idea leave you with as a client?

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
    <tr><td><strong>Criterion 1 - Separation Efficiency</strong></td><td>Count SLF models remaining entangled with grapes before and after a 60-second agitation cycle</td><td>≥90% of SLF models successfully separated</td><td>High</td></tr>
    <tr><td><strong>Criterion 2 - Processing Throughput</strong></td><td>Stopwatch timing from when the user touches the lid to when the grapes are ready for the next stage</td><td>≤4 minutes per 1kg batch</td><td>Medium</td></tr>
    <tr><td><strong>Criterion 3 - Operating Stability</strong></td><td>Pre- and post-spin position markings on the table plus graduated cylinder to measure spilled water</td><td>≤2cm of movement, ≤50ml lost at maximum RPM</td><td>Medium</td></tr>
  </tbody>
</table>
</div>

**Exhibit Day Demo:** We will present a 3D-printed bucket pre-filled with water and a contaminated batch of grape and SLF models. After a 30-second agitation cycle, we will pour the cleaned grapes into a transparent bowl to visually show separation, then weigh the recovered SLF models on a small scale to demonstrate Criterion 1 is met in real time.

### Design Intent

The prototype is a water-based agitation system driven by a handheld drill. The core functional components are:

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component</th><th>Material</th><th>Function</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Agitator Bucket</strong></td><td>3D-printed PLA</td><td>A sealed container that holds water, grape models, and SLF models. Acts as the stationary outer vessel during operation.</td></tr>
    <tr><td><strong>Shaft</strong></td><td>Machined aluminum (Al 6061)</td><td>Transfers rotational motion from the drill down into the bucket. A flange at the top constrains vertical movement, and the shaft rotates freely relative to the bucket. Connected to the agitator head via press fit.</td></tr>
    <tr><td><strong>Agitator Head</strong></td><td>3D-printed PLA</td><td>A propeller/paddle assembly press-fit onto the bottom of the shaft. When spun, it agitates the water, creating turbulence that causes low-density SLF models to float while denser grape models sink.</td></tr>
    <tr><td><strong>Legs</strong></td><td>3D-printed PLA</td><td>Columns that provide enough clearance between the floor and the bottom of the bucket for the drill to fit in.</td></tr>
  </tbody>
</table>
</div>

Additionally, grape and SLF models were made to test separation.

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Model</th><th>Material</th><th>Specifications</th><th>Density Target</th></tr>
  </thead>
  <tbody>
    <tr><td><strong>Grape Models</strong></td><td>3D-printed PLA</td><td>Spheres with diameter of 20mm and weight of 4.61g</td><td>~1.1 g/cm³</td></tr>
    <tr><td><strong>SLF Models</strong></td><td>3D-printed PLA</td><td>Cylinders with diameter 10mm, height 5mm, and weight of 1.42g</td><td>~1.0 g/cm³</td></tr>
  </tbody>
</table>
</div>

### Assembly Instructions

1. **Prepare the Shaft** - Insert the machined aluminum shaft through the center hole of the Agitator Bucket. The flange at the top of the shaft should seat flush against the rim of the bucket, constraining the shaft from dropping through.
2. **Attach the Agitator Head** - Press-fit the Agitator Head onto the top of the shaft inside the bucket. Ensure the fit is firm with no rotational play. The agitator head should sit near the bottom of the bucket without contacting the bucket floor.
3. **Verify Clearance** - Rotate the shaft by hand to confirm the agitator head spins freely without scraping the inner walls of the bucket. Minimum clearance should be maintained on all sides (reference Test 2 data: 4.86 inches measured).
4. **Connect the Legs** - Insert three legs into the three bottom holes near the circumference of the bucket. The fit should be tight.
5. **Connect the Drill** - Insert the end tip of the shaft into the drill chuck. Tighten securely. The drill should be able to drive the shaft in both clockwise and counterclockwise directions for oscillating agitation.
6. **Load the Bucket** - Fill the Agitator Bucket with water to the marked fill line. Add the grape models and SLF models to the water.
7. **Operate** - Power the drill, toggling direction every ~2 seconds to simulate oscillating agitation. Run for 30-60 seconds. SLF models should migrate to the water surface while grape models remain submerged.

### Design Tests

#### Test 1: Comparing the effectiveness of agitation with single-direction spinning

**What is being tested:** The effectiveness of the propeller's constant change of direction vs single-direction spinning in separating grapes and SLF models.

**How it was tested:**
- Place a known mixture (10 grape models and 10 SLF models) into the container of water
- Run the drill for 30 seconds using a single-direction spin
- Repeat the test with a new mixture, but manually toggle the drill direction every 2 seconds to simulate an agitator
- Visually assess the separation of SLF and grapes, taking images. Count how many SLF models have successfully floated/separated from the grape cluster in each scenario

**What happened:** Both directions of agitation showed similar amounts of separation; however, the oscillating mechanism led to a greater success rate among 10 trials.

**Quantitative metrics:**

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Metric</th><th>Single Direction</th><th>Bi-Directional</th></tr>
  </thead>
  <tbody>
    <tr><td>Avg Separation %</td><td>79.5%</td><td>84.5%</td></tr>
    <tr><td>Time to first separation</td><td colspan="2">3.78 sec ± 0.15 seconds (from each of the 20 trials)</td></tr>
  </tbody>
</table>
</div>

<div class="highlight-box">
  <strong>Design Change Needed:</strong> Since bi-directional agitation is significantly more effective, we need to design a mechanical linkage or use a programmable motor controller to automate the direction switching rather than relying on a manual drill trigger.
</div>

#### Test 2: Propeller Cavitation & Turbulence Range

**What is being tested:** Determining whether the propeller creates enough "lift" to move the SLF models without hitting the bucket walls or the grapes themselves.

**How it was tested:**
- Fill the bucket to a marked "fill line" and operate the propeller at 25%, 50%, and 75% power
- Observe the "vortex depth" (the distance from the water surface to the lowest point of the whirlpool)
- Measure the distance (in mm) between the spinning propeller tip and the inner wall of the 3D-printed bucket to check for dynamic clearance

**What happened:** The drill was run at 75%, 50%, and 25% power by marking how far the trigger traveled. Using a custom 3D-printed measuring tool, 2 trials on each of the three speeds were conducted.

**Quantitative metrics:**
- Clearance from walls: 4.86 inches
- Spillage: Low, with only a few drops being spilled

<div class="warning-box">
  <strong>Design Change Needed:</strong> We must increase the diameter and size of our propeller since the vortex is both low in depth and has an incredibly small width. By scaling the vortex up around 2.2x its original size, we were able to conduct the nice separation test from above. In addition, we need to make the propeller's workholding a larger diameter, as in the course of these tests, around 3 propellers broke and needed replacement.
</div>

#### Test 3: Structural Integrity & Fastening (The "Drill-to-Propeller" Joint)

**What is being tested:** Assembly and fastening to ensure the connection between the drill bit and the 3D-printed propeller doesn't slip or strip under the resistance of the water.

**How it was tested:**
- Perform a cycling test of 20 cycles, each lasting 30 seconds
- Between each cycle, attempt to manually wiggle the propeller on the shaft to check for loosening
- Inspect the 3D-printed "socket" for signs of permanent deformation or cracking

**What happened:** After 20 cycles (30 seconds of spinning), the propeller developed slight rotational play and minor wear inside the 3D-printed socket, but no cracking occurred.

**Quantitative metrics:**
- Cycles completed: 20 cycles of 30 seconds, no breakage, but increased vibration/chatter in the final 5 cycles
- Connection play in mm developed after 20 cycles: 2.7 mm (measured via bore caliper, comparing the original socket diameter to the new one)

<div class="highlight-box">
  <strong>Design Change Needed:</strong> If the propeller begins to slip on the drill shaft, we will iterate the design to ensure a more secure mechanical lock between the motor and the agitator.
</div>

#### Test 4: Leak test

**What is being tested:** How much water is lost through the basket.

**How it was tested:**
- Fill the basket with water to the highest level
- For 1 minute, count the number of droplets that leave the basin
- Repeat the test 3 times

**What happened:** Water was filled to the fill line, paper towels were placed underneath the base for better accuracy, and a minute was timed on the stopwatch.

**Quantitative metrics:**

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Trial</th><th>Drops Lost</th><th>Water Loss (ml/minute)</th></tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>11</td><td>0.55 ml</td></tr>
    <tr><td>2</td><td>7</td><td>0.35 ml</td></tr>
    <tr><td>3</td><td>14</td><td>0.70 ml</td></tr>
  </tbody>
</table>
</div>

<div class="highlight-box">
  <strong>Design Change Needed:</strong> While the TPU shaft seal holds water incredibly well, better tolerancing on our 3D prints and machine shaft and perhaps an actual shaft seal from McMaster-Carr will truly make this a watertight machine.
</div>

---

## Client Report

**Team Name:** F4 Pest Control  
**Team Members:** Liz Tipton, Katelyn Fu, Arda Griffin, Sarah Bulkley, Junseok Kang  
**Date:** May 5, 2026

### Context and Problem Statement

Invasive Spotted Lanternflies (SLF) pose a significant $8.8 million threat to the regional grape population [1]. National food regulations mandate that SLF be removed before final production. Currently, entire batches of harvested grapes are often discarded if contamination is found. Our team focused on a post-harvest solution that leverages the physical density differences between the insects and the fruit to ensure crop viability and consumer safety.

<div class="highlight-box">
  <strong>Primary constraint:</strong> The primary constraint was to achieve a separation efficiency of at least 90% to meet industrial standards.
</div>

### Final Prototype and Application

We developed a water-based mechanical agitation system. The grapes contaminated with SLF are placed in the basin, and the mixture is agitated with the propeller, facilitating consistent and effective separation. SLF rise to the surface, and grapes sink due to their varying densities.

<div class="success-box">
  <strong>Result:</strong> Achieving a 93% separation efficiency, exceeding our initial 90% goal.
</div>

This prototype is intended for use at the initial stage of grape processing, where harvested batches can be submerged and agitated to quickly remove invasive pests.

### Testing and Results

#### Test 1: Identifying Optimal RPM

The primary objective of the product is to separate SLF from grapes. We wanted to test at what RPM separation is most effective. In previous testing, we identified that single-directional spinning was more effective than bi-directional agitation. In this test, we aim to refine our separation method.

**Results:** Observed that at low RPM (~3000 RPM), the majority of grape models sink, and SLF models get the most effectively separated at 3000 RPM. As the RPM increases above the 3000-4000 range, grape models do not effectively sink and float with SLF models due to the excessively strong vortex created by the agitation. The highest separation efficiency of 93% is reached at approximately 3000 RPM.

#### Test 2: Leak Test

The design must be able to hold water without significant leakage since the separation mechanism relies on water to separate the grapes from the SLF.

We tested the four most leak-prone areas in our design.

**Results:**

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Leak-Prone Area</th><th>Area 1</th><th>Area 2</th><th>Area 3</th><th>Agitator</th>
  </thead>
  <tbody>
    <tr><td>Number of Water Drops observed within one minute of submersion</td>
    <td>0</td><td>0</td><td>0</td><td>15</td>
  </tr>
</tbody>
</table>
</div>

No leak through the gap between the three side wall parts (Area 1, 2, 3) suggesting that using sealant and glue to connect the sides was sufficient. However, there was a noticeable leak through the center of the product (Area 4), where the shaft and bearing are. After the results we added more sealant below the base, which reduced leakage. The results suggest that the interface between the agitator and the base requires a redesign.

### Conclusion and Recommendation

The functional prototype successfully demonstrated a 93.3% separation efficiency, exceeding our initial target of 90%.

**For industrial scaling:** The side walls should be manufactured as a singular unit to eliminate seam-related leak risks. Future iterations must utilize a motor capable of maintaining a constant 3,000 RPM under load. Materials should be transitioned to plastics or metals that will not corrode after long-term exposure to water and acidic grape juice. Other considerations include food safety. Although RTV sealant is food-safe, as is PETG, the lubricant we used around the shaft as well as the glue used to hold the side walls together is not suitable for use in food production.

**Shortcomings:** Since the design uses very few commercially available components, most manufacturing would have to be custom, increasing the per-unit cost. If scaled up, a mechanism would have to be put in place to extract the SLF once they rise to the top and extract the grapes when they sink. The current prototype was only designed with testing efficiency of separation in mind. Another shortcoming of the design is potential loss of harvest. Without draining, grape juice is lost when it is diluted with water, so systems would have to be put in place to preserve as much of the harvest as possible. So despite high separation efficiency, a redesign is required if the design is to be used on an industrial scale.

### Prototype and Testing Details

The device consists of the agitator housed within a baseplate and three side walls. A motor spins the agitator at speeds up to 7000 RPM. The prototype utilizes a standard ASME press-fit for the metal-to-plastic interface of the agitator. The agitator interfaced with the baseplate through the use of a bearing and o-ring assembly.

In order to prevent leaks, RTV sealant was used around each of the side walls and the base. RTV sealant was chosen for its vibration resistance and water-blocking properties.

**Testing methodology for separation efficiency:** To model the SLF and grapes we used 3D-printed models that were accurate to the density shown in the image. SLF models (cylinders) with density 1g/cm³ and grape models (spheres) with density 1.1g/cm³ [3,4].

We placed 10 SLF models and 10 grape models into the container and ran the motor at varying RPMs ranging from 500 to 7000. For each of the three trials per RPM we ran the motor for 30 seconds and then counted the number of SLF that floated to the surface (NSLF float) and the number of grapes that sunk (Ngrapes sunk).

Then we calculated separation efficiency using the following formula:

<code style="background: #f5f5f5; padding: 2px 6px; border-radius: 4px;">Separation efficiency = (NSLF float + Ngrapes sunk) / 20</code>

**Testing methodology for leak test:** Each leak-prone area was submerged each for 1 minute using an arbitrary controlled amount of water and the number of drops was counted.

**Test for Structural Integrity and Fastening:** In addition to a leak test and a test for separation efficiency, we also tested the structural integrity of the connection between the motor shaft and the agitator. One key safety concern is that the agitator head must not come loose from the motor shaft during testing.

**Methodology:** To test the connection we performed a cycling test of 20 cycles, each lasting 30 seconds, and then inspected the attachment between the motor shaft and the agitator for signs of loosening.

**Results:** After several tests, the shaft started spinning within the agitator without causing the agitator to spin. To combat this, we used a quick-setting epoxy adhesive, after which there were no more issues with adhesion between the agitator and the motor.

### Bill of Materials

**3D-Printed Components**

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component Name</th><th>Description</th><th>Quantity</th><th>Total Cost (USD)</th></tr>
  </thead>
  <tbody>
    <tr><td>Side Walls</td><td>Three 3D-printed pieces connect to the baseplate. Grape and SLF mixture are contained here.</td><td>3</td><td>$25.36</td></tr>
    <tr><td>Agitator</td><td>Consists of a 3D-printed propeller and shaft that fit into the motor.</td><td>1</td><td>$2.84</td></tr>
    <tr><td>Baseplate</td><td>3D-printed plate where the side walls attach to. Houses bearing and o-ring to prevent leakage.</td><td>1</td><td>$12.85</td></tr>
    <tr><td>Stand</td><td>3D-printed stand that houses the motor and speed controller.</td><td>1</td><td>$35.25</td></tr>
  </tbody>
</table>
</div>

**Off-the-Shelf Components (OTS)**

<div class="table-wrapper">
<table>
  <thead>
    <tr><th>Component Name</th><th>Description</th><th>Quantity</th><th>Total Cost (USD)</th></tr>
  </thead>
  <tbody>
    <tr><td>Ball Bearing</td><td>Circular ball bearing reduces friction when the agitator is being spun.</td><td>1</td><td>$28.17</td></tr>
    <tr><td>Spring-loaded O-ring</td><td>Reduces leakage around the agitator shaft.</td><td>1</td><td>$4.98</td></tr>
    <tr><td>Motor</td><td>High Torque DC Motor 12V/24V. 30W CW/CCW 3500/7000RPM</td><td>1</td><td>$22.99</td></tr>
    <tr><td>Speed controller</td><td>DC Motor Speed Controller PWM Controller</td><td>1</td><td>$12.73</td></tr>
    <tr><td>Power Supply</td><td>24V 3A Power Supply 72W, 24 Volt DC Power Adapter with On/Off Switch</td><td>1</td><td>$13.85</td></tr>
    <tr><td>Sealing Hex Head Screw 1/4-20</td><td>Used to connect the side walls to the baseplate.</td><td>6</td><td>$15.06</td></tr>
    <tr><td>1/4-20 Nut</td><td>Used together with bolts.</td><td>6</td><td>$0.76</td></tr>
    <tr><td>1/4-20 Heat Insert for plastic</td><td>Fused into the stand, allowing a connection between the side walls, the base plate, and the stand.</td><td>6</td><td>$2.40</td></tr>
    <tr><td>RTV Sealant Aluminum Color</td><td>Used to seal connections for waterproofing. RTV sealant was chosen for its vibration resistance and water-blocking properties.</td><td>1</td><td>$12.89</td></tr>
  </tbody>
</table>
</div>

### References

1. Cornell University News. "Spotted Lanternflies Could Cost NYS Grape Industry Millions." Jan 2025.

2. United States Department of Agriculture. "United States Standards for Grades of Grapes for Processing and Freezing." Sept 1977. Reprinted Jan 1997.

3. Zuritz, C. et al. (2005). "Density, viscosity and coefficient of thermal expansion of clear grape juice." *Journal of Food Engineering*, 71, 143-149.

4. Kühsel, S. et al. (2016). "Surface area - volume ratios in insects." *Insect Science*, 24.