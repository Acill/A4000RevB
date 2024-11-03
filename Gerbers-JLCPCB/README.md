# Gerber Files with the New Silkscreens
Original Gerber files were created Using Mentor PADS application. When imported to most PCB production house websites, like JLCPCB.com, several layers are not shown correctly and will not be aligned to each other. I had a set of PCBs produced at JLC. They made the necessary adjustments and produced the boards correctly. As part of the process, they provided adjusted Gerber files. Those files are shown correctly when opened by any Gerber viewer. I imported those files into Kicad and completely redid the silkscreens on both sides.

Note that the Kicad files I created cannot be used to modify the copper and other production related layers as original component information is lost and all layers were converted to graphical elements.

As part of the production process, JLCPCB makes an adjustment to drill holes (slightly enlarge them). As we are using adjusted files, they should not do another adjustment on them. Make sure to add the note below as part of PCB remarks.

PCB Remark:
Drill layer was already compensated and optimized. Do not further modify drill layer values.

# Updated Pick and Place Files
I updated the BOM and CPL files to fix placement and rotation issues. Some of the parts are not available in JLCPCB stocks and must be ordered via Global Parts service. These orders usually take 2-3 weeks to arrive to your inventory at JLCPCB. Some parts are too expensive or not available even from GP service partners. These parts are not listed in the BOM file but they are still listed in the CPL file in case you wish to get them populated. As a result, when importing BOM/CPL files, you will get a warning about some missing parts in BOM file. Just accept and continue.

U700 (Super Buster) and U714 (GAL) sockets cannot be assembled at the same time as they have a slight conflict. I chose to get U700 socket populated by JLCPCB and slightly shave and hand solder U714 socket.

Some of the PLCC sockets show location pins when there is no hole for them on the PCB. JLCPCB PCBA team will ask you whether they should cut the pins of the PLCC socket at a cost. The part numbers I have in the BOM do not have those location pins, so there is nothing to cut. Give them this response and you will be fine. There is a PCBA remark box when ordering, but they ignored and asked me anyway.

PCBA Remark:
SMD PLCC sockets used in this project do not have placement pins. Ignore the holes or hole markers on the PCB for PLCC sockets and use pin 1 indicator on the silkscreen for the orientation of the sockets.

Kavanoz, May 2024

Preview of new Gerbers

![Gerber-Viewer-Top](https://github.com/kavanoz64/A4000RevB/assets/45491268/0ce9b232-56a8-4c60-983f-a9036568ef47)

![Gerber-Viewer-Bottom](https://github.com/kavanoz64/A4000RevB/assets/45491268/a30536cc-f61f-42fc-be1f-9b431be66ee9)

Actual assembled PCB as produced by JLCPCB (There have been a slight update on the silkscreens after these were ordered)
![Acill A4000D-Kavanoz-Top](https://github.com/kavanoz64/A4000RevB/assets/45491268/19b7a3a4-fcac-43ac-ace7-4eebed84f8a4)

![Acill A4000D-Kavanoz-Bottom](https://github.com/kavanoz64/A4000RevB/assets/45491268/8514268a-7d6b-420d-af0f-d33664c9fdc0)
