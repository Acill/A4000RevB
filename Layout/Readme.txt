Please review the attached PADS PCB database.
The design has been updated and follows the schematic netlist exactly.
To view the plane data go to 'Tools' and then the 'Pour Manager', 'Plane Connect' and pour all. 

This is similar to the original trace routing but I update to be more manufacturable.
The best I could do in regards to design rules, is with the majority of the board at 10mil traces and 8mil space.  Power and ground at 20mil.
Some areas have 6 mil spacing and 8 mil lines.
Unfortunately this was a poorly designed board in terms of maufacturability.  It should have been a 6 layer board.
The biggest issue is with the trace routing and trying to fit the large number of signal connections on only 2 layers.  
The original designers put traces between the pads of the SM resistors and capacitors, not generally a good idea.
Trace entry to pads was very poor with lots of 'acid traps'.
There were a few dead traces and extra vias.  At some point some of the vias may have been used as test points(?).

At least it is better than the original at this point.  I did not move the parts but cleaned the traces and changed via types.
I you want to make the board to IPC specifications at some point,  we would need to go to 6 layers and redefine most of the SM parts.
