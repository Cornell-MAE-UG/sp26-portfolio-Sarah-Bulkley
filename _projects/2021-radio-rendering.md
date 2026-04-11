---
layout: project
title: Spotted Lanternfly Mechanical Separator
description: Design Project
technologies: [Autodesk Fusion]
image: /assets/images/radio-machine-cad.jpg
---
---
layout: project
title: Spotted Lanternfly Mechanical Separator
description: Design Project
technologies: [Autodesk Fusion]
#image: /assets/images/radio-machine-cad.jpg
---

## 📋 Table of Contents
{: .no_toc}

* TOC
{:toc}

---
## Client Pitch
Team: Pest Control Clients: Cornell CALS Extension / E&J Gallo Winery / National Grape 
Problem: Viticulturalists in New York State are affected by the spotted lantern fly infestation, an invasive species that contaminates the harvest. Batches are rejected from juiceries and wineries, resulting in economic loss. Traditional pest-control methods are insufficient. Pesticides come with high economic and environmental costs. Egg removal proves too difficult because of the massive scale of laying locations, costing too much in labor. 
Impact: Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting the growing consumer demand. 

Solution: Centrifugal Density Separator- A high-speed rotation device that separates harvested grapes from SLF by density, removing them from the desired product. 
How to implement: Harvest is loaded into the device, and an internal drum spins at a calculated RPM. Heavier grapes are pushed out furthest, sliding down the angled outer walls into a collection bin. Lighter insects get pulled into a secondary bag. This way, grape pulp is conserved without contamination. 
Why it’s better than the status quo: Pesticides leave a taint on the wine’s taste profile and contaminate the organic integrity of the grapes. Manual sorting is slow, costly, and prone to human error/inconsistencies. Our solution is non-chemical and efficient on a large scale.
End-of-semester proof-of-concept: A benchtop rotating drum prototype using grapes and 3D printed SLF accurate to weight and size, allowing us to optimize RPM. Success is determined by comparing the percentage of pests (SLF models) successfully sorted with the percentage of harvest lost.
Key risks/unknowns:
Damage to grapes: A high RPM exerts a force on the grape skin, possibly causing the grapes to break apart. Assessing the damage to grapes requires a physical "Burst Test," spinning grapes at incremental RPMs to identify when skins rupture, then comparing our results to the RPM needed to separate SLF.
Mass variation and obstructions: While a dry lanternfly is less dense than a grape, a lanternfly soaked in grape juice is much denser. Similarly, an SLF wedged inside a tight cluster might not separate easily, resulting in less effective separation. We can test this by using "weighted" objects (3D-printed bugs with adhesive, SLF tucked inside dense clusters or higher-density SLF), measuring SLF removed per cycle at various degrees of obstruction.
Processing time: A centrifuge is often a batch process, and if the device takes too long to load, spin, and unload, farmers will reject it in favor of faster methods. To address this, we will test the time the cycle duration of our prototype, and calculate the throughput to compare it to standard manual sorting speeds.
Questions for the client
How much material other than grapes, like stems and leaves, typically remains in the bin after your primary harvest? This changes our separation threshold and testing parameters based on what we want to separate/how much grapes weigh.
What is the maximum holding time allowed between the grape being picked and it reaching the crusher before you worry about quality loss? This determines the constraints of our time trials and whether or not our product is viable in the time scale of grape processing.
Do the SLF tend to stay on the surface of the grape clusters when disturbed, or do they retreat deep into the center of the bunch? This affects the “ramping profile” (i.e. how fast we accelerate) based on how hard SLF tends to stay on grapes, and also how we simulate SLF in our separation experiments.
What reservations does this idea leave you with as a client? (Any issues we haven’t thought of?)
References:
Penn State Agricultural Division. “Spotted Lanternfly.” Penn State Extension, extension.psu.edu/spotted-lanternfly.
Penn State Agricultural Division, “Spotted Lanternfly Management in Vineyards.” Penn State Extension, extension.psu.edu/spotted-lanternfly-management-in-vineyards.
Department of Environmental Conservation, NYS. “Spotted Lanternfly - NYDEC.” Dec.ny.gov, 16 Mar. 2017, dec.ny.gov/nature/animals-fish-plants/spotted-lanternfly.

## Functional Prototype

Success Criteria

Context: Our device helps grapevine farmers mechanically separate invasive Spotted Lanternflies (SLF) from harvested grapes using water-based agitation and density-driven buoyancy.
Criterion 1 – Separation Efficiency (High Priority): Assesses whether the device reliably floats SLF models away from grape clusters. 
Measurement: Count SLF models remaining entangled with grapes before and after a 60-second agitation cycle. 
Target: ≥90% of SLF models successfully separated.
Criterion 2 – Processing Throughput (Medium Priority): Assesses whether the device is fast enough for practical farm use. 
Measurement: Stopwatch timing from when the user touches the lid to when the grapes are ready for the next stage. 
Target: ≤4 minutes per 1kg batch.
Criterion 3 – Operating Stability (Medium Priority): Assesses whether the device stays safe and controlled during operation. 
Measurement: Pre- and post-spin position markings on the table (target: ≤2cm of movement) and a graduated cylinder to capture spilled water (target: ≤50ml lost at maximum RPM).
Exhibit Day Demo: We will present a 3D-printed bucket pre-filled with water and a contaminated batch of grape and SLF models. After a 30-second agitation cycle, we will pour the cleaned grapes into a transparent bowl to visually show separation, then weigh the recovered SLF models on a small scale to demonstrate Criterion 1 is met in real time.

Design intent
The prototype is a water-based agitation system driven by a handheld drill. The core functional components are:
Agitator Bucket – A sealed 3D-printed PLA container that holds water, grape models, and SLF models. It acts as the stationary outer vessel during operation.
Shaft – A machined aluminum (Al 6061) rod that transfers rotational motion from the drill down into the bucket. A flange at the top constrains vertical movement, and the shaft rotates freely relative to the bucket. Connected to the agitator head via press fit.
Agitator Head – A 3D-printed PLA propeller/paddle assembly press-fit onto the bottom of the shaft. When spun by the drill, it agitates the water, creating turbulence that causes low-density SLF models to float while denser grape models sink.
Legs – 3D-printed PLA columns that provide enough clearance between the floor and the bottom of the bucket for the drill to fit in.
Additionally, grape and SLF models were made to test separation.
Grape Models – 3D-printed PLA parts sized, shaped, and weighted to replicate the density and surface geometry of real grapes. Spheres with a diameter of 20mm and a weight of 4.61g.
SLF Models – 3D-printed PLA parts sized, shaped, and weighted to simulate the density and surface geometry of real Spotted Lanternflies. Cylinders with diameter 10mm, height 5mm, and weight of 1.42g.

Assembly instructions
Step 1 – Prepare the Shaft Insert the machined aluminum shaft through the center hole of the Agitator Bucket. The flange at the top of the shaft should seat flush against the rim of the bucket, constraining the shaft from dropping through.
Step 2 – Attach the Agitator Head Press-fit the Agitator Head onto the top of the shaft inside the bucket. Ensure the fit is firm with no rotational play. The agitator head should sit near the bottom of the bucket without contacting the bucket floor.
Step 3 – Verify Clearance Rotate the shaft by hand to confirm the agitator head spins freely without scraping the inner walls of the bucket. Minimum clearance should be maintained on all sides (reference Test 2 data: 4.86 inches measured).
Step 4 – Connect the Legs. Insert three legs into the three bottom holes near the circumference of the bucket. The fit should be tight.
Step 5 – Connect the Drill. Insert the end tip of the shaft into the drill chuck. Tighten securely. The drill should be able to drive the shaft in both clockwise and counterclockwise directions for oscillating agitation.
Step 6 – Load the Bucket. Fill the Agitator Bucket with water to the marked fill line. Add the grape models and SLF models to the water.
Step 7 – Operate. Power the drill, toggling direction every ~2 seconds to simulate oscillating agitation. Run for 30–60 seconds. SLF models should migrate to the water surface while grape models remain submerged.

Design Tests

Test 1: Comparing the effectiveness of agitation with single-direction spinning
What is being tested: 
The effectiveness of the propeller’s constant change of direction vs single-direction spinning in separating grapes and SLF models
How it was tested:
Place a known mixture (10 grape models and 10 SLF models) into the container of water.
Run the drill for 30 seconds using a single-direction spin.
Repeat the rest with a new mixture, but manually toggle the drill direction every 2 seconds to simulate an agitator.
Visually assess the separation of SLF and grapes, taking images. Count how many SLF models have successfully floated/separated from the grape cluster in each scenario
What happened: Both directions of agitation showed similar amounts of separation; however, the oscillating mechanism led to a greater success rate among 10 trials. There are 10 of each, grape and SLF, represented by their densities and general surfaces in 3D printed form, in each of 10 trials, (see the table below) the oscillating mechanism performed marginally better and with less variance.
Quantitative metrics: 
Avg Separation % for Single Direction Spinning (#Flown/Sunk over total): 79.5% 
Avg Separation % for Bi-Directional (#Flown/Sunk over total): 84.5% 
Time to first separation: 3.78 sec ± 0.15 seconds (from each of the 20 trials)
Design Changes Needed: 
Since bi-directional agitation is significantly more effective, we need to design a mechanical linkage or use a programmable motor controller to automate the direction switching rather than relying on a manual drill trigger.

Test 2: Propeller Cavitation & Turbulence Range
What is being tested: 
Determining whether the propeller creates enough "lift" to move the SLF models without hitting the bucket walls or the grapes themselves
How it was tested: 
Fill the bucket to a marked "fill line" and operate the propeller at 25%, 50%, and 75% power.
Observe the "vortex depth" (the distance from the water surface to the lowest point of the whirlpool).
Measure the distance (in mm) between the spinning propeller tip and the inner wall of the 3D-printed bucket to check for dynamic clearance.
What happened: 
The drill was run at 75,50,25 percent power by marking how far the trigger traveled and (assuming it was proportional to the drill's power/speed) running the experiment while the trigger is pulled to its respective mark. Using a custom 3d printed measuring tool (that was tiny enough not to disturb the vortex, 2 trials on each of the three speeds were conducted (see data below). Because of the nature of our oscillations being inconsistent and often breaking the vortex, only single-directional vortices were measured
Quantitative metrics: 
Vortex Depth in cm at different % of power.
Clearance from walls: 4.86 inches
Spillage. Low, with only a few drops being spilled onto the paper tower
Design Changes Needed: 
We must increase the diameter and size of our propeller since the vortex is both low in depth and also has an incredibly small width. By scaling the vortex up almost around 2.2X its original size, we were able to conduct the nice separation test from above. In addition, we need to make the propellers' workholding a larger diameter, as in the courses on these tests, around 3 propellers broke and needed replacement.

Test 3: Structural Integrity & Fastening (The "Drill-to-Propeller" Joint)
What is being tested: 
Assembly and fastening to ensure the connection between the drill bit and the 3D-printed propeller doesn't slip or strip under the resistance of the water.
How it was tested: 
Perform a cycling test of 20 cycles, each lasting 30 seconds.
Between each cycle, attempt to manually wiggle the propeller on the shaft to check for loosening.
Inspect the 3D-printed "socket" for signs of permanent deformation or cracking
What happened: 
After 20 cycles (30 seconds of spinning), the propeller developed slight rotational play and minor wear inside the 3D-printed socket, but no cracking occurred.
Visual Inspection: Shining a light perpendicular to the surface of the socket, you can visually inspect the gap from how much light goes through, and hits our shaft seal and reflects the TPU coating. Comparing the before and after, we could visually see more of the TPU shaft seal than before.
Quantitative Metrics: 
Cycles completed: 20 Cycles of 30 seconds, no breakage, but increased vibration/chatter in the final 5 cycles.
Connection Play in mm developed after 20 cycles. 2.7 mm (measured via bore caliper, comparing the original socket diameter to the new one)
Design Changes Needed: If the propeller begins to slip on the drill shaft, we will iterate the design to ensure a more secure mechanical lock between the motor and the agitator.


Test 4: Leak test
What is being tested: 
How much water is lost through the basket.
How it was tested: 
Fill the basket with water to the highest level.
For 1 minute, count the number of droplets that leave the basin
Repeat the test 3 times
What happened: Water was filled to the fill line, paper towels were placed underneath the base for better accuracy, and a minute was timed on the stopwatch.
Quantitative Metrics: 
Number of drops lost in each cycle (list): 11,7,14
Average rate of water loss (ml/minute) = #drops*0.05ml/1min = 0.55 ml, 0.35 ml, 0.7 ml
Design Changes Needed: While the TPU shaft seal holds water incredibly well, better tolerancing on our 3D prints and machine shaft and perhaps an actual shaft seal from McMaster Carr will truly make this a watertight machine.
