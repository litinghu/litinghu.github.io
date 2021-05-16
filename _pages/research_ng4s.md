---
title: "Elves Lab - Research_ng4s"
layout: textlay
excerpt: "Elves Lab -- Research_ng4s"
sitemap: false
permalink: /research_ng4s/
---

# NG4S: A Next-generation Geo-distributed Scalable Stateful Stream Processing System

## Project Summary

<p>Our society increasingly relies on applications that process streaming data across geo-distributed sites, such as making business decisions from marketing data, identifying spam campaigns in social network streams, and analyzing genome datasets in different labs and countries to track the sources of potential epidemics. Existing systems are mainly designed for stateless stream processing in intra-datacenter settings and do not scale well for running stream applications that contain large distributed states. This project breaks the traditional abstractions of a centralized architecture and hashtable-based stateless operators, redefining them with a new decentralized architecture and new memory-efficient stateful operators, which enables novel approaches to improve overall system performance and scalability.</p>

<p>This project includes three primary research directions. (1) At the architecture layer, a new decentralized 'many masters/many workers' architecture is proposed to provide each master with maximum independence. (2) At the operator layer, a new in-memory data structure is proposed to store the application state that minimizes the memory overhead. (3) At the mechanism layer, a new shard-based parallel recovery mechanism is proposed to handle failures and stragglers. All three parts of the project will be prototyped and implemented on real-world stream processing systems.</p>

## Participants

<h3 style="text-indent: 0.5em">Principal Investigator</h3>

- Dr. Liting Hu, Assistant Professor, Virginia Tech
- Dr. Dilma Da Silva, Professor, Texas A&M University

<h3 style="text-indent: 0.5em">Members</h3>

- Hailu Xu, Ph.D. student, Florida International University
- Pinchao Liu, Ph.D. student, Florida International University
- Boyuan Guan, Ph.D. student, Florida International University
- Susana Cruz-Diaz, B.S. student, Florida International University
- Ulises Fernandez, B.S. student, Florida International University

## Publications

- <b>[USENIX ATC'21]</b> Pinchao Liu\*, Dilma Da Silva, Liting Hu, \"DART: A Scalable and Adaptive Edge Stream Processing Engine\", in <em>Proceedings of the 2021 USENIX Annual Technical Conference (USENIX ATC'21)</em>, July 2021. Acceptance Rate: 64/341 = 18.8%.
- <b>[Middleware'20]</b> Hailu Xu*, Pinchao Liu*, Susana Cruz-Diaz*, Dilma Da Silva, Liting Hu, \"SR3: Customizable Recovery for Stateful Stream Processing Systems\", in <em>Proceedings of ACM/IFIP Middleware 2020 (Middleware'20)</em>, December 2020.
- <b>[IPDPS'20]</b> Pinchao Liu\*, Hailu Xu\*, Dilma Da Silva, Qingyang Wang, Sarker Tanzir Ahmed, Liting Hu, \"FP4S: Fragment-based Parallel State Recovery for Stateful Stream Applications\", in <em>Proceedings of the 34th IEEE International Parallel & Distributed Processing Symposium (IPDPS'20)</em>, May 2020.
- <b>[Cloud'19]</b> Hailu Xu\*, Pinchao Liu\*, Boyuan Guan\*, Liting Hu, \"Exploiting the Spam Correlations in Scalable Online Social Spam Detection\", in <em>Proceedings of the 2019 International Conference on Cloud Computing (Cloud'19)</em>, June 2019. Best Student Paper Award

## Presentations

FP4S: Fragment-based Parallel State Recovery for Stateful Stream Applications <br />
IPDPS'20 <br />
[Slides]() <br />

Pinchao Liu, SR3: Customizable Recovery for Stateful Stream Processing Systems <br />
Middleware'20 <br />
[Slides](https://drive.google.com/file/d/10UH2LZ-ZnzRZRunomaLmW0WXol24bMGD/view?usp=sharing) <br />
<iframe width="560" height="315" src="https://youtu.be/4ElTxy9YVFE" frameborder="0" allowfullscreen></iframe>

## Source Code

- DART: A Scalable and Adaptive Edge Stream Processing Engine [[Source Code]](https://github.com/fiu-elves/DART)

## Outreach

Curriculum Development Activities
- Course 6913: Advanced Topics in Information Processing. [[Video Playlist Link]](https://www.youtube.com/watch?v=fhN3szbOr9E&list=PLGtMEQgQy8UZvqmsXzeJ43Xzm_ItCQekE)

Stream Processing Tutorials
- [Apache Storm](https://youtu.be/-8XGburfkuY)
- [Apache Flink](https://youtu.be/wLJHhZs4bTU)
- [Apache Storm Encoding](https://youtu.be/Yc-YfVANAeY)


## Acknowledgement

<p>This material is based upon work supported by the National Science Foundation SPX award  NSF-SPX-1919126 and  NSF-SPX-1919181.</p>