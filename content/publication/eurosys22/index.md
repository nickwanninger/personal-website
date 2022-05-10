---
title: Isolating Functions at the Hardware Limit with Virtines
subtitle: ""
publication_types:
  - "1"
authors:
  - admin
  - Joshua Bowden
  - Kirtankumar Shetty
  - Ayush Garg
  - Kyle Hale
publication: EuroSys 2022
publication_short: EuroSys'22
abstract: An important class of applications, including programs that leverage
  third-party libraries, programs that use user-defined functions in databases,
  and serverless applications, benefit from isolating the execution of untrusted
  code at the granularity of individual functions or function invocations.
  However, existing isolation mechanisms were not designed for this use case;
  rather, they have been adapted to it. We introduce virtines, a new abstraction
  designed specifically for function granularity isolation, and describe how we
  build virtines from the ground up by pushing hardware virtualization to its
  limits. Virtines give developers fine-grained control in deciding which
  functions should run in isolated environments, and which should not. The
  virtine abstraction is a general one, and we demonstrate a prototype that adds
  extensions to the C language. We present a detailed analysis of the overheads
  of running individual functions in isolated VMs, and guided by those findings,
  we present Wasp, an embeddable hypervisor that allows programmers to easily
  use virtines. We describe several representative scenarios that employ
  individual function isolation, and demonstrate that virtines can be applied in
  these scenarios with only a few lines of changes to existing codebases and
  with acceptable slowdowns.
draft: false
url_pdf: /papers/eurosys22.pdf
featured: true
tags:
  - Virtualization
  - Execution Environments
categories: []
projects: []
summary: ""
lastmod: 2022-05-09T22:01:04-05:00
date: 2022-05-09T22:01:04-05:00
links:
  - name: ACM DL
    url: https://dl.acm.org/doi/abs/10.1145/3492321.3519553
url_code: https://github.com/virtines/wasp
---
