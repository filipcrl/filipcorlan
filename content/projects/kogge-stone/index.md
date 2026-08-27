+++
title = "Full-Custom 64-Bit Accumulator"
description = "A showcase of my first large custom design"
date = 2026-08-25

[taxonomies]
categories = ["Projects"]
tags = ["design"]

[extra]
image = "cover.png"
+++

Over the course of the autumn semester, I designed a 64-bit accumulator, iterating on the schematic and completing the layout, post-layout extraction, and simulation. One interesting aspect of the design is its use of dynamic p-n domino logic, which enables higher maximum speeds than traditional CMOS logic. However, this requires routing the clock to every logic gate, making clock skew more critical. To address this, I created an H-tree-style clock network placed between each pair of tiles that make up the accumulator.

![Kogge-Stone topology](/projects/kogge-stone/image.png)

Overall, this project helped me better understand digital design by allowing me to work at a lower level of abstraction. Because the Kogge-Stone adder has many global connections across its individual slices, the project particularly helped me understand the challenges of routing and how it can become a design bottleneck.
