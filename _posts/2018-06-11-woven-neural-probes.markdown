---
layout: post
title:  "Woven Neural Probes"
date:   2018-06-11 17:40:06
categories: Bioengineering
tags:
- implants
- medical devices
image: wnp/sma-cover.jpg
description: Flexible neural implants using muscle wire. Click to read more.  
---

![Woven mesh using muscle wire (SMA).](/assets/images/wnp/sma-cover.jpg "Mesh before coated in PEG."){: .center-image}

<br>

Recently, scientists are reaching the limit of data that can be collected about the brain. If we want to do things like computational analysis, and neural net models, we are going to need much more data from individual neurons. At the BioSensing and BioRobotics lab, I helped develop affordable, flexible, neural probes for neurological research.

Chronic implamentation further adds additional engineering issues. Implants physically shift, causing additional damage to tissue, and loosing signal quality with the original neuron it landed on. Scientists can only keep track of, and reposition so many neurons before severe tissue damage, or losing track of each neuron happens.

<br>

**Technical** 

---

<br>

All versions of the tetrode wiring use SANDVIK tetrode wire (link here) with 0.0001” diameter. The wire consists of a highly conductive metal, with a thin coating of polyimide inssulanting the length of the wire. For SMA, we used wires from Flexinol (link here) ranging from 0.005”-0.001” diameter. Due to limited availability, all experiments used SMA wire that actuated at 70 degrees celcius. In reality, custom SMA wire with an actuation temperature closer to body temp will be used.

Tetrode wire, which is a thin, highly conductive wire coated with a polyimide coating (purchase here) was used to pick up signals. Shape-memory alloy (SMA), also known as ‘muscle wire’, was purchased from Flexinol (here) in various lengths. Due to limited material availability, we used SMA wire that actuated at 70 degrees celcius. Various combinations of combining SMA and tetrode implant wired were tried.

Due to the poor/insufficient binding, we swithed to one using a woven loom. A piece of 1/8” - thick acrylic was cut on a laser cutter in the pattern shown below. (below post a pictoral representation of the mesh, labeling holes for weaving and other important items). In previous experiments, my coworkers designed, etched, and got manufactured a circuit board to connect with computer.

SMA wire was first woven into the desired pattern. Then, tetrode wire is woven throught the electrical connectors at the top of the circuit board, ending at the rest of the mesh. Once weaving was done, and all wires were taught, adhesive was carefully applied where SMA and tetrode wire crossed. To remove the mesh from the weaving jig, scissors were used to cut the SMA, then the tetrode.

<br>

**Result**

---

<br>

After ten trials, and one major design shift, we were able to successfully have a neural mesh expand in agar once heat was applied.

{% include image.html
            img="/assets/images/wnp/wnp-exp-chart.png"
            title="Basic summary of tests we did."
            caption="Basic summary of tests we did." %}

<br>

**Review**

---

<br>

What went well:

- SMA was able to fully expand the mesh in the air
- The initial mesh PEG coating proved stiff enough to enter the brain.
- SMA successfully actuated in agar substitute

Not so hot:

- In order to test quickly, we had to use off-the-shelf SMA wire. The best wire for testing, unfortunately had an activation temperature of ~70 degrees celcius. The higher temperature meant that during testing, the agar also changed characteristics slightly.
- Despite trying multiple adhesives, all proved to have problems with controlling the amount dispensed onto the mesh. 
- Weaving jigs were one-time use. 