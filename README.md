# Advanced Physical Design 

## Table of Contents
<h3>Part 1: Inception of open-source EDA, OpenLANE and Sky130 PDK</h3>
1. How to talk to computers
2. SoC design and OpenLANE
3. Starting RISC-V SoC Reference design
4. Get familiar to open-source EDA tools

<h3>Part 2: Good floorplan vs bad floorplan and Introduction to library cells</h3>

1.Chip Floor planning considerations
2.Library Binding and Placement
3.Cell design and characterization flows
4.General timing characterization parameters

<h3>Part 3: Design library cell using Magic Layout and Ngspice characterization</h3>

1.Labs for CMOS inverter ngspice simulations
2.Inception of Layout – CMOS fabrication process
3.Sky130 Tech File Labs

<h3>Part 4: Pre-layout timing analysis and importance of good clock tree</h3>

1.Timing modelling using delay tables
2.Timing analysis with ideal clocks using openSTA
3.Clock tree synthesis TritonCTS and signal integrity
4.Timing analysis with real clocks using openSTA

<h3>Part 5: Final steps for RTL2GDS using OpenSTA</h3>

1.Routing and design rule check (DRC)
2.PNR interactive flow tutorial


## Introduction
This project is a product of the 5 day workshop conducted by VLSI Sstem Design on Advanced Physical Design. The focus is to complete the RTL to GDSII flow for PicoRV32 which is RISCV based core. The following steps will be carrried out:
+ Synthesis
+ Floorplan
+ Placement
+ Clock Tree Synthesis
+ Routing

## Tools Used
All tools used in this project are open sourced
+ OpenLANE: It is an automated RTL to GDSII (Registered Transfer Level to Graphic Data System version II) flow that is built on top of several open source tools, aiming to be a fully automated ASIC (Application-Specific Integrated Circuit) flow. OpenLANE is intended to produce clean GDSII without any human intervention, although, there is an interactive mode available to allow for custom modifications and design tuning. The OpenLANE flow involves several stages, including synthesis, floorplanning, placement, routing, and checking for manufacturability (DRC). Here's a brief overview of these stages:

  - **Synthesis:** The input RTL design (in Verilog, for instance) is transformed into a gate-level representation. Yosys is the tool used for this.

  - **Floorplanning:** Arrangement of macro blocks and determining the shape and size of the chip. OpenROAD is one of the tools used for this.

  - **Placement:** Determines the exact location of standard cells in the layout. OpenROAD is again the tool used for this.

  - **Routing:** The interconnections between the cells are created, forming a complete network of paths for the design.

  - **DRC (Design Rule Checking):** The final layout is checked against a set of design rules to ensure it can be accurately manufactured.
 
 
+ SKY130 PDK: The Sky130 Process Design Kit (PDK) is a significant offering from SkyWater Technology. It's known as the world's first manufacturable, open-source PDK. A PDK (Process Design Kit) is essential for chip design as it describes how a particular fabrication technology can be used for designing integrated circuits. SkyWater's Sky130 PDK provides a 130-nanometer fabrication process that can be used to design a wide range of ICs (Integrated Circuits). It is particularly notable because of its open-source nature. Prior to the release of Sky130 PDK, virtually all PDKs were proprietary, making this a major step towards enabling open-source hardware and democratizing IC design. Key aspects of the Sky130 PDK include:
  - **130-nanometer process:** The 130nm process allows for reasonable performance and power levels while remaining accessible for smaller design teams.
  
  - **Open-source:** The Sky130 PDK is open-source and available for anyone to use. This is a major departure from traditional PDKs, which are typically proprietary.
  
  - **Versatility:** The Sky130 PDK is suitable for a wide range of designs, including mixed-signal and analog, radio frequency (RF), and ultra-low power applications.
  
  - **Manufacturable:** The Sky130 PDK is not just a theoretical or educational tool; it can be used to create designs that can actually be manufactured by SkyWater's foundry services.
  
  
+ Magic: Magic is a venerable VLSI (Very-Large-Scale Integration) layout tool, written in the 1980s at the University of California, Berkeley. It is widely known in academia for its interactive mode, which allowed designers to directly manipulate design layouts. Key Features of Magic:

  + **IC Layout:** Magic is a key tool in designing the layout of integrated circuits (ICs) in VLSI.

  + **Technology-Agnostic:** It is adaptable to various IC fabrication technology rules, such as SCMOS, and has been updated for deep sub-micron designs.

  + **Interactive:** Magic is not just a drawing tool, it's an intelligent layout editor. As the user manipulates the design layout, Magic continuously performs design rule checking (DRC) to ensure that the layout obeys the specific rules of the fabrication process.

  + **Extensible:** Magic is extensible and has been used as a base for several IC design automation tools.

  + **CIF and GDS Conversion:** Magic supports CIF (Caltech Intermediate Form) and GDS (Graphic Data System) formats, which are common formats for IC design files.

  + **Open Source:** Magic is open-source software, which means it's freely available for use and modification.

While Magic is quite old compared to many of today's EDA (Electronic Design Automation) tools, it is still used in education and research due to its ease of use, interactive capabilities, and extensibility.

+ Ngspice
+ OpenSTA



## Methodology
<h2>Part 1: Inception of open-source EDA, OpenLANE and Sky130 PDK</h2>

<h2>Part 2: Good floorplan vs bad floorplan and Introduction to library cells</h2>
```git 

git clone some repo
```

![All the config files](/workspaces/physical_design_openlane/Images/2_all_config_files.png)
![All the config files](/workspaces/physical_design_openlane/Images/2_all_config_files.png)
<h2>Part 3: Design library cell using Magic Layout and Ngspice characterization</h2>
<h2>Part 4: Pre-layout timing analysis and importance of good clock tree</h2>
<h2>Part 5: Final steps for RTL2GDS using OpenSTA</h2>

![All the config files](Images/2_all_config_files.png)
<h2>Part 3: Design library cell using Magic Layout and Ngspice characterization</h2>
<h2>Part 4: Pre-layout timing analysis and importance of good clock tree</h2>
<h2>Part 5: Final steps for RTL2GDS using tritonRoute and OpenSTA</h2>

## Acknowledgements

This project wouldn't have been possible without the help of:

- [Kunal Ghosh](https://github.com/kunalg123) - Co-founder VSD Corp. Pvt. Ltd 
- [Nickson Hose](https://github.com/nickson-jose/) - Teaching Assistant VSD Corp. Pvt. Ltd) (link to their GitHub or website)
