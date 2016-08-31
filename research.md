---
layout: page
title: Research
menu: true
---
# Research Projects
[Energy Efficient Data Movement](#eedm)

----------------------------------
#### <a href="#eedm"> </a> Energy Efficient Data Movement

My primary research seeks to address the challenges in improving the energy efficiency of data movement in computing systems. It has become increasingly clear as we develop more energy-efficient compute units to combat power constraints that data communication dominates overall energy both within a single chip and to external memory. To retain the energy efficiency of emerging compute accelerators we have to reduce the amount of data moved per operation. Today, an L1 cache access consumes as much pJ as a floating point operation; supplying the operands even from the local cache cost as much in picojoules as a floating point operation; supplying data from caches further away on the chip can cost up to 300x more energy. 


Another challenge posed to the memory system is the increasing heterogeneity: the number of specialized compute units increased from 9 to 27 progressing from the Apple A4 to A8. As applications migrate across the chip seeking the most energy-efficient compute unit introducing further challenges to minimize the communication energy. I believe that it is imperative to optimize data movement and retain a coherence-based memory model that implicitly moves data between the compute units helping the programmer deal with the increased complexity in the compute units. 


<img src="{{ site.baseurl }}/public/images/research_triangle.jpg class="img-responsive img-rounded" style="width:400">

My focus has been to develop more energy efficient hardware caches and coherence protocols that adapt to application characteristics and minimize data movement. The enclosed figure summarizes my primary research agenda since 2011; to move data around the chip efficiently i) we reduced the distance the data has to traverse by localizing communication and proactively moving the compute closer to the data, ii) we reduced the number of data bits moved by developing message-free coherence protocols and by eliminating untouched data from the caches, and iii) finally, we reduced the data access cost improving the efficiency of caches.
