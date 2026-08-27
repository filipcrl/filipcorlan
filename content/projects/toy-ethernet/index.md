+++
title = "Toy Ethernet (WIP)"
description = "A project for improving my understanding of networking"
date = 2026-07-20

[taxonomies]
categories = ["Projects"]
tags = ["fpga", "networking"]

[extra]
image = "cover.png"
+++

I started this project to improve my understanding of computer networking, particularly Ethernet. The source code is available in the [toyethernet repository](https://github.com/filipcrl/toyethernet).

I am currently implementing a TCP server in Python, building the network stack from the data link layer upward and exposing it through a virtual network interface. Ethernet and IPv4 support are complete. The TCP server is still in progress, but it can receive data sent through Netcat while keeping track of TCP sequence numbers.

Once the Python implementation is complete, I plan to build a TCP server module for FPGAs. It will use AXI4-Stream input and output interfaces and build on the open-source [verilog-ethernet](https://github.com/alexforencich/verilog-ethernet) project for Ethernet and IP support.
