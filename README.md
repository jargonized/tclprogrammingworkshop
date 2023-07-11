# TCL WORKSHOP - Introduction to Advanced Scripting Techniques in Design and Synthesis

![Workshop Banner](/docs/workshop_banner.jpg)

# About

A comprehensive 5 day training workshop that is designed to ignite your passion for TCL and equip you with the skills needed to excel in advanced scripting techniques required in the realm of EDA. 

Workshop conducted by VLSI System Design : [VSD website](https://www.vlsisystemdesign.com/)

# Outline

1. [Introduction](#1-introduction)
2. [Synth Toolbox](#2-synth-toolbox)
2.1 [Usage Scenario 1](#21-usage-scenario-1)
2.2 [Usage Scenario 2 & 3](#22-usage-scenario-2-and-3)
3. [Variable Creation](#3-variable-creation)
4. [Processing constraints from the CSV File](#4-processing-constraints-from-the-csv-file)
5. [Processing clock constraints](#5-processing-clock-constraints)
6. [Processing input constraints](#6-processing-input-constraints)
7. [Processing output constraints](#7-processing-output-constraints)
8. [Yosys](#8-yosys)
9. [Hierarchy Check](#9-hierarchy-check)
10. [Synthesis using Yosys](#10-synthesis-using-yosys)
11. [Procs](#11-procs)
12. [Netlist and SDC processing for Opentimer](#12-netlist-and-sdc-processing-for-opentimer)
13. [Static Timing Analysis (STA) and Quality of Results (QOR)](#13-static-timing-analysis-sta-and-quality-of-results-qor)
14. [Conclusion](#14-conclusion)

[Acknowledgement](#acknowledgement)

[Bibliography](#bibliography)

# 1. Introduction

The name Tcl is derived from "Tool Command Language" and is pronounced "tickle". Tcl is a radically simple open-source interpreted programming language that provides common facilities such as variables, procedures, and control structures as well as many useful features that are not found in any other major language.

For Electronic Design Automation (EDA) applications, TCL has emerged as the de facto industry standard embedded command language. TCL is the ideal option if you need to automate repetitive behavior, expand an application’s capabilities, manage many tools with a single script, or develop a unique GUI.

In this report, a TCL toolbox is created to process a verilog design. Design details and constraints were extracted and the design was synthesised using Yosys. The synthesis output and the SDC were further processed to be fed into the OpenTimer tool for Static Timing Analysis (STA). The prelayout STA results were inferred from the results file and printed to the user.
 
# 2. Synth Toolbox

| ![files](docs/w%20(2).png) |
|:--:|
| Fig. 1 Creation of vsdsynth file amd addition of first line for shell scripting |

| ![files](docs/w%20(1).png) |
|:--:|
| Fig. 2 Verifying the creation of file using vim |

| ![files](docs/w%20(4).png) |
|:--:|
| Fig. 3 Making the file executable and checking the acccess modification |
 
## 2.1 Usage Scenario 1

| ![files](docs/w%20(3).png) |
|:--:|
| Fig. 4 Script to check if a file is provided|

| ![files](docs/w%20(5).png) |
|:--:|
| Fig. 5 Checking both use cases - file not given and file given |

## 2.2 Usage Scenario 2 and 3

| ![files](docs/w%20(7).png) |
|:--:|
| Fig. 6 Scripts for scenario 2 - user invoking help menu - and scenario 3 - user providing a CSV file that does not exits|

| ![files](docs/w%20(6).png) |
|:--:|
| Fig. 7 Verification of scenarios 2 and 3|

# 3. Variable Creation 
 
| ![files](docs/w%20(9).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(8).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(11).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(12).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(13).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(14).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(15).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(16).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(17).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(18).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 4. Processing constraints from the CSV File

| ![files](docs/w%20(19).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(20).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(21).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(22).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(23).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(24).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(25).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(26).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(27).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 5. Processing clock constraints

| ![files](docs/w%20(28).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(29).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(30).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(31).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 6. Processing input constraints

| ![files](docs/w%20(32).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(33).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(34).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(36).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 7. Processing output constraints

| ![files](docs/out_sdc_sc.png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(37).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(38).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(39).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 8. Yosys

Yosys is the first full-featured open source software for Verilog HDL synthesis. It supports most of Verilog-2005 and is well tested with real-world designs from the ASIC and FPGA world.

Synthesis using Yosys can be well understood from [my report here](https://github.com/jargonized/sky130RTLDesignandSynthesisWorkshop)

# 9. Hierarchy Check

| ![files](docs/w%20(40).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(41).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(42).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(43).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(44).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(45).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(46).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(47).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(48).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 10. Synthesis using Yosys

| ![files](docs/w%20(49).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(50).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(51).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(52).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(53).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(54).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 11. Procs

| ![files](docs/w%20(59).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(60).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(61).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(62).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(63).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(64).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(65).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(66).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(67).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(68).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 12. Netlist and SDC processing for Opentimer

| ![files](docs/w%20(55).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(56).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(57).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(58).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 13. Static Timing Analysis (STA) and Quality of Results (QOR)

| ![files](docs/w%20(69).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(70).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(71).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(73).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(72).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(75).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|
 
| ![files](docs/w%20(76).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

| ![files](docs/w%20(74).png) |
|:--:|
| Fig. 79 Generation of LEF (Library Exchange Format) file|

# 14. Conclusion

# Acknowledgement

The above work was carried out as a part of the 5-day workshop on TCL Programming organised by VLSI System Design. I am greatly indebted to Kunal Ghosh (course instructor), Geetima Kachari (TA) and the entire VSD Team for this great learning experience and immense guidance provided throughout the workshop.

# Bibliography

1. [TCL in VLSI](https://chipedge.com/tcl-scripting-for-vlsi-a-brief-guide/#:~:text=TCL%20(Tool%20Command%20Language)%20is,tools%20are%20built%20on%20it.)
2. 

