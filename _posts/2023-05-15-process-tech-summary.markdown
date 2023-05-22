---
layout: post
comments: true
title:  "Life of a semiconductor chip: Conception to Tapeout"
excerpt: "A journey of what it takes to get a commerical semiconductor chip built."
category: blog
permalink: /blog/chip-design-cycle
date:   2023-03-15 10:00:00
mathjax: false
---

<style>
p {
  text-align: justify;
}
.post pre, .post code {
    border: none;
    background-color: #eee;
}

</style>


Coming out of college, students often do not understand the lifecycle of a chip from ideation to its eventual tapeout. I was definitely one of them! This is quite understandable since chip design information can be quite opaque, and the processes have massively matured beyond what school can teach. Given that semiconductors have been becoming increasingly important for deep learning (and national security!), we will go over an overview of what it takes to do that. 

Disclaimer:
1. Most of the steps below overlap to some extent, if not completely. The objective is to disentangle the steps or "parallel processes" to help highlight the nuances.
2. Not every company will follow the steps exactly. Depending on the target market (automotive, 5G, healthcare) and the maturity of the company (startup vs big), companies might do only a subset of the steps, or add a few more. But the hope is to highlight the most common steps.

<hr style="border:none; height:1px; background-color: #333;">
<!-- <br> -->

#### Table of Contents
1. [Architecture Exploration](#architecture-exploration)
2. [Design Execution](#design-execution)
3. [Verification](#verification)
4. [Physical Design](#physical-design)
5. [QoR Tuning](#qor)
6. [Emulation and Tapeout](#emulation-and-tapeout)

### Architecture Exploration
When we build a chip, we basically want to provide a computing platform to the end user with useful *features*. The feature can be provided either in hardware or software. Hardware features are those which have hardware acceleration. Specifically, the chip has transistors that does a specific function when given the appropriate command or instruction. Software features are software programs (API, packages etc. ) that make it easier to use the hardware either for performance, usability or efficiency. The architecture exploration phase is used to determine what new features we want in hardware or software (or the compiler too, in recent times).

Given that we are basically doing research for the next generation of the chip, we want to be able to develop a framework which guides our direction and decisions. Let us look at some important considerations of this framework.
- **Pain points of previous/other chips** : 
- **Market** : Different markets like datacenters, graphics, automotive and healthcare will have specific needs. Given the subset of markets we want to target, the features will need to be general enough to help all necessary domains, or we might need different features for different markets. 
- **Customers** : Some customers might have very specific needs. If a particular customer is particularly important to you, then you have to balance between satisfying the customer's request and your long term vision. 
- **Compatibility** : 
- **Development time** : 
- **Cost** : 

### Design Execution
### Verification
### Physical Design 
### QoR Tuning
### Emulation and Tapeout
