---
layout: post
title:  "Soft Robotics"
date:   2017-5-8 17:40:06
categories: hardware
tags:
image: claw-v2-all.jpg
description: Manufacturing soft robots using cheaper materials. Click to read more.
---

![Claw v2 trimmed](/assets/images/claw-v2-trimmed.jpg "It looks like icing"){: .center-image}

<br>

Soft robotics have the potential to provide inexpensive, versatile, safe use in conjunction with humans. Materials to manufacture these robots, however, can be cost-prohibitive, especially with low-volume production. While researching materials, I came across an [Instructables post](https://www.instructables.com/id/How-To-Make-Your-Own-Sugru-Substitute/) on how to create a sugru substitute. Using corn starch and silicone caulk, the person created a sticky, yet flexible material for gluing and mounting items. I wanted to see if this forumla has sufficient properties to replace two-part silicone moulding compound in robotics applications. 

<br>

**Technical**

---

<br>

I quickly wanted to get testing, so I used this [four arm gripper](https://www.instructables.com/id/Air-Powered-Soft-Robotic-Gripper/) based on research from Harvard.[^1]. The mould is filled with material and left to dry, while additional material is spread onto a flat surface, creating an elastic pancake. Once dried, the mould and the pancake are sealed together using additional compound. A tube is inserted into the central chamber. When pressure is applied, the orientation of the various air chambers cause the claw to close.

The mould was printed with black PLA using the following settings:

- Infill: 12%
- outer perimeters: 3
- extruder temperature: 245 degrees celsius
- bed temperature: 60 degrees celsius

{% include image.html
	img="/assets/images/mould-v1-printing.jpg"
	title="printing"
	caption="The first mould was printed at too high of a temperature" %}

<br>

When the mould finished printing, wispy strands of PLA were left over from filament oozed out of the nozzle during non-printing movement. With a knife, I removed as much of the stringing as possible. 

Per the directions, I combined approximately 12 pumps of silicone caulk, with a heaping tablespoon of cornstarch. Two things became apparent:

1. Silicone caulk smells like awfully strong vinegar.
2. Adding the cornstarch turned the silicone into a paste that's has to be spooned into the mould. I didn't have a syringe large enough to extrude the paste, meaning that it's more likely air gaps would appear in the casting. 

<br>

{% include image.html
	img="/assets/images/claw-v1-underside.jpg"
	title="the first casting"
	caption="The first casting. Note the bits of PLA (black spots), and how the paste wasn't fully compacted into the mould." %}

<br>
{% include image.html
	img="/assets/images/claw-v2-underside.jpg"
	title="the second casting"
	caption="The second casting turned out much better." %}

<br>

As shown above, the silicone wasn't pressed down hard enough. Another mould was printed, this time with machine changes listed below:

1. Temperature was lowered.
2. Retraction enabled at 0.2 mm.
3. Nozzle wiping enabled to 0.6 mm.
4. Cooling fan raised to 100% speed. 

The second casting proved suitable for use. 
<br>

**Result**

---

<br>

{% include image.html
				img="/assets/images/claw-v2-all.jpg"
				title="the second version of the claw"
				caption="The second casting of the claw." %}

<br>

When I applied pressure through the syringe, the entire claw swelled, then a weak spot in the silicone gave way, breaking the seal. 

<br>

{% include image.html
	img="/assets/images/claw-v2-blowout.jpg"
	title="claw blowout"
	caption="A thin portion of the claw's underside blew out when pressure was applied." %}


<br>

**Review** 

---

<br>

What went well:
- Silicone mixture casted fairly well.
- Resulting gripper was somewhat flexible.

Not so hot:
- I did not have a degasser to completely remove air bubbles when casting the gripper.
- The silicone mixture didn't flow easily; I had to pack down the mixture into the mould. 

<br>

---

<br>

[^1]: licensed under the Creative Commons - Attribution - Non-Commercial license. The mould STL file can be found [here](http://www.thingiverse.com/thing:66883).




