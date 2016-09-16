---
layout: post
title: "Accelerator Benchmarks"
tags: [accelerators]
---

At IISWC 2016 (the premier conference on workloads) my group will be releasing SPEC-AX and PARSEC-AX, benchmark suites for hardware accelerators. 

In computer systems and architecture, typically we do not get to make real progress until we develop a benchmark suite to help us understand the target problems at hand and help compare design alternatives. Benchmarking is a key tool for assessing computer systems. A key benefit of benchmarks is to enable comparing design alternatives during research or development and evaluating power/performance tradeoffs

Recent papers at ISCA, MICRO, and ASPLOS have produced dozens of accelerators and it is challenging to compare these accelerator designs since even if they target the same workload they may not be targetting the same program behavior or code region. Furthermore it is not clear how can one begin to even think about leveraging these accelerators for their own problem. Computer architects have truly run amok with specialization; effectively we are writing "specialized" papers in which every paper is targetting a specific code region in a specific application. How then can we draw lessons and progress as a field?


"Hardware accelerators" have introduced a chicken-and-egg problem;  designing accelerators suitable for applications requires the applications to convey  precisely what function needs to be accelerated in the first place. Our work seeks to explore accelerators in existing CPU-based applications and make it possible for architects and designers to rapidly explore behaviors to specialize and accelerate. We ensure that the accelerators developed for the demarcated regions within each application can be directly deployed within the original application. Furthermore, accelerators developed for a workload are all targetting the same code region.









