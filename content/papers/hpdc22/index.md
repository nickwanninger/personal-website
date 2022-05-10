---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "FPVM: Towards a Floating Point Virtual Machine"
subtitle: ""
summary: ""
authors:
  - Peter Dinda
  - admin
  - Jiacheng Ma
  - Alex Bernat
  - Charles Bernat
  - Souradip Ghosh
tags:
  - Virtualization
  - Execution Environments
categories: []
date: 2022-05-09T22:01:04-05:00
lastmod: 2022-05-09T22:01:04-05:00
featured: false
draft: false

# url_pdf: '/papers/eurosys22.pdf'
# url_code: 'https://github.com/virtines/wasp'
# links:
# - name: ACM DL
#   url: https://dl.acm.org/doi/abs/10.1145/3492321.3519553

projects: []
---

Alternatives to IEEE floating point arithmetic have become all the rage. Some extract more representational power out of the avail- able bits. Others offer the potential for lower or higher precision than is available in IEEE-compatible hardware. Even an “interface to the real numbers” has recently been proposed. Using such al- ternative arithmetic systems within an existing scientific or other significant codebase is a major challenge, however. We explore how to address this challenge through virtualizing the IEEE float- ing point hardware, specifically on x64. The goal of the floating point virtual machine (FPVM) is to allow an existing application binary to be seamlessly extended to support the desired alternative arithmetic system with overheads determined by that system and not the virtualization mechanisms. We describe the prospects, is- sues, and tradeoffs for four different approaches for building FPVM: trap-and-emulate, trap-and-patch, binary transformation, and IR transformation. We then describe the design and implementation of our current design, which combines static binary analysis/trans- lation and trap-and-emulate execution. We evaluate our FPVM implementation on several benchmarks, virtualizing them to use posits and MPFR. Finally, we comment on kernel- and hardware- level innovations that could further reduce overheads for floating point virtualization.