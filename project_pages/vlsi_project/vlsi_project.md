---
layout: inner
title: Low-Power SRAM
permalink: /low-power-sram/
---
# 1 Mbit Ultra-Low Power SRAM
*This project was completed as part of ECE 4332 (Introduction to VLSI Design) at UVA*


### Project Goals
<p class="description">The goal of this project was to design a 1 Mbit SRAM and implement the design using FreePDK's 45nm technology in Cadence Virtuoso, while demonstrating functionality at the following PVT corners:</p>

<ul>
    <li>[TT, FF, SS, FS, SF]</li>
    <li>[0C, 27C, 50C]</li>
    <li>[VDD - 10%, VDD, VDD + 10%]</li>
</ul>

<p class='description'>The design was to be optimized such that the following figure of merit was minimized:</p>

$$ (Active\ energy\ per\ access)^2(Delay)(Area)(Idle\ Power)$$

### Approach
<p class='description'>The figure of merit equation guided my approach to this design. Since $V_{DD}$ is squared in the active energy equation, which is itself then squared in the design metric, lowering $V_{DD}$ was given the highest priority when making design decisions. I also sought to reduce the active energy per access by structuring large interconnects hierarchically and looking for energy-optimized bitcells in the literature.</p>

### Outcomes

<p class='description'> <b> Design Outcomes </b></p>
<ul>
    <li>We achieved a figure of merit of $ 2.05 \times 10^{-33} J^2*sec*mm*W$, whereas the historical class average is on the order of $10^{-29}$</li>
    <li>We measured an extremely low average energy per access of $687$ fJ for the read operation and $875$ fJ for the write operation at $50$ MHz and $V_{DD}=0.4\ V$.</li>
    <li>We recorded an inactive power of $123\ \mu W$ under 27C, TT conditions.</li>
</ul>

<p class='description'> <b> Skill-related Outcomes </b></p>
<ul>
    <li>Practiced self-pacing a months-long project with little direction beyond specification (e.g., setting internal deadlines, putting roadmap into place at beginning of semester) </li>
    <li>Honed communication skills when team was not working harmoniously by coordinating and mediating a meeting between team members. Generated action items to help course-correct and improve collaboration, ultimately leading to a successful project delivery</li>
    <li>Improved ability to evaluate design space and make decisions at all levels of system hierarchy to tailor design to application needs</li>
    <li>Gained experience with schematic capture in Cadence Virtuoso and design verification using Spectre</li>
    
</ul>

### Report
<p class='description'>For more details about the project, check out the report embedded below.</p>

<div class='pdf-container'>
<object data="../../assets/DesmanECE4332Report.pdf" style="width:100%;height:100%;" type='application/pdf'></object></div>




