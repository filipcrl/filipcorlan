+++
title = "FPGA Test Board Showcase"
description = "A showcase of a breakout board I designed to test a custom sensor chip"
date = 2026-08-03

[taxonomies]
categories = ["Projects"]
tags = ["pcb", "fpga"]

[extra]
image = "cover.png"
+++

The picture shows a test board that I designed during my time as a research assistant in the [AQUA laboratory](https://www.epfl.ch/labs/aqua/) at EPFL. It will be used to test the functionality of a custom chip consisting of an array of time-to-digital converters.

When stacked with an array of silicon photomultipliers, the chip will be able to timestamp the arrival of photons very accurately. This technology will be used to build better PET scanners.

## Board Design

The board includes an arbitrary low-jitter clock generator to drive the chip. To distinguish between events at different energy levels, it also features a low-latency, high-speed ADC connected to the FPGA. In addition, the board has adjustable power supplies and a high-speed transimpedance amplifier for sensing current pulses from the photomultipliers.

The board is designed to be used with the XEM7360 module from Opal Kelly, which we use to interface with the chip via USB. I am currently updating my old FPGA design to work with this new board and integrate its new features.
