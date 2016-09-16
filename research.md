---
layout: page
title: Research
menu: true
---
- [Hardware Accelerators](#accel)
- [Energy Efficient Data Movement](#eedm)
- [Text Processing](#text)

***************
#### <a href="#eedm"> </a> Hardware Accelerators

Accelerators promise software developers orders-of-magnitude improvement in energy efficiency and performance, provided software developers can develop techniques to build accelerators for their applications. Typically, software engineers were not required to know the details of the hardware design during application development. However, the gaining prevalence of custom hardware motivates us to explore solutions to enable software engineers to reason about opportunities for using customized hardware and to effectively participate in the definition and utilization of such accelerators. Our research effort is a step in this direction focusing on techniques to help programmers mine the information about the software and use them to develop efficient acceleratable code which in turn will be used to guide the design of the accelerator. 

<img src="{{ site.baseurl }}/public/images/Accelerator.jpg" class="img-responsive img-rounded" style="width:400px"> 

Extracting accelerators requires software developers to grasp, what code regions work well in hardware?, what might be the power and performance benefits of accelerating such regions?, What is the specific behavior that is being accelerated? In the past, these questions have been arguably more challenging since they required the creation of large-enough acceleratable code sections to offset the communication costs. Today, closer on-die integration of FPGAs into the cache hierarchy increases the scope of acceleration. We will address a key challenge for accelerators: how to increase the fraction of program code offloaded to the accelerator without losing the benefits of the run- time and energy from specialization for a small frac- tion. Applications include complex control flow and have many execution paths making it challenging to profile and compose an offload region for the acceler- ator. As such, our proposed research will take a ver- tical cut through the system stack and address chal- lenges at the programming level, system software and performance monitoring level and system integration and abstraction. 


----------------------------------
#### <a href="#eedm"> </a> Energy Efficient Data Movement

My primary research seeks to address the challenges in improving the energy efficiency of data movement in computing systems. It has become increasingly clear as we develop more energy-efficient compute units to combat power constraints that data communication dominates overall energy both within a single chip and to external memory. To retain the energy efficiency of emerging compute accelerators we have to reduce the amount of data moved per operation. Today, an L1 cache access consumes as much pJ as a floating point operation; supplying the operands even from the local cache cost as much in picojoules as a floating point operation; supplying data from caches further away on the chip can cost up to 300x more energy. 


Another challenge posed to the memory system is the increasing heterogeneity: the number of specialized compute units increased from 9 to 27 progressing from the Apple A4 to A8. As applications migrate across the chip seeking the most energy-efficient compute unit introducing further challenges to minimize the communication energy. I believe that it is imperative to optimize data movement and retain a coherence-based memory model that implicitly moves data between the compute units helping the programmer deal with the increased complexity in the compute units. 


<img src="{{ site.baseurl }}/public/images/research_triangle.jpg" class="img-responsive img-rounded" style="width:400px"> 


My focus has been to develop more energy efficient hardware caches and coherence protocols that adapt to application characteristics and minimize data movement. The enclosed figure summarizes my primary research agenda since 2011; to move data around the chip efficiently i) we reduced the distance the data has to traverse by localizing communication and proactively moving the compute closer to the data, ii) we reduced the number of data bits moved by developing message-free coherence protocols and by eliminating untouched data from the caches, and iii) finally, we reduced the data access cost improving the efficiency of caches.

----------------------------------
#### <a href="#eedm"> </a> Text Processing Analytics

Along with my student Dan Lin, and colleague, Rob Cameron, I have been working on Parabix, a domain specific language and programming framework for streaming text processing applications, leveraging both SIMD and multicore processubg. The Parabix framework is based on the concept of parallel bit streams, a fundamentally new transform representation of text. Byte-oriented character stream data is first transformed into eight parallel bit streams, each bit stream comprising one bit per character code unit. We have developed an XML parser and regular-expression search using the framework and demonstrated up to a 5x speedup compared to existing systems. We have published our work at HPCA'12, PACT'14, and XML-Balisage'14.
