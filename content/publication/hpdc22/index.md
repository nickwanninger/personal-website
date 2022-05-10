---
title: "FPVM: Towards a Floating Point Virtual Machine"
subtitle: ""
publication_types:
  - "1"
authors:
  - Peter Dinda
  - admin
  - Jiacheng Ma
  - Alex Bernat
  - Charles Bernat
  - Souradip Ghosh
publication: HPDC 2022
publication_short: HPDC'22
abstract: "Alternatives to IEEE floating point arithmetic have become all the
  rage. Some extract more representational power out of the avail- able bits.
  Others offer the potential for lower or higher precision than is available in
  IEEE-compatible hardware. Even an “interface to the real numbers” has recently
  been proposed. Using such al- ternative arithmetic systems within an existing
  scientific or other significant codebase is a major challenge, however. We
  explore how to address this challenge through virtualizing the IEEE float- ing
  point hardware, specifically on x64. The goal of the floating point virtual
  machine (FPVM) is to allow an existing application binary to be seamlessly
  extended to support the desired alternative arithmetic system with overheads
  determined by that system and not the virtualization mechanisms. We describe
  the prospects, is- sues, and tradeoffs for four different approaches for
  building FPVM: trap-and-emulate, trap-and-patch, binary transformation, and IR
  transformation. We then describe the design and implementation of our current
  design, which combines static binary analysis/trans- lation and
  trap-and-emulate execution. We evaluate our FPVM implementation on several
  benchmarks, virtualizing them to use posits and MPFR. Finally, we comment on
  kernel- and hardware- level innovations that could further reduce overheads
  for floating point virtualization."
draft: false
featured: false
tags:
  - Virtualization
  - Floating Point
categories: []
projects: []
summary: ""
lastmod: 2022-05-09T22:01:04-05:00
date: 2022-05-09T22:01:04-05:00
---
