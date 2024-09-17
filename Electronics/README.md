## To order using JLCPCB
1. Clone or download the repository
2. Zip all files in the PCB Gerbers folder
3. Upload the zip on JLCPCB
4. Use the default settings, except for:
    1. Set "Mark on PCB" to "Remove mark"
    2. Set "PCB Color" to whatever you prefer
    3. Enable the PCB Assembly option
        1. PCBA Type: Economic
        2. Assembly Side: Top Side
        3. Tooling holes: Added By Customer
        4. Parts Selection: By Customer
5. In the assembly wizard, you need to upload a BOM and CPL file:
BOM file is: Electronics\PCB Components\ESPkamstrup-BOM-JLCPCB.csv
CPL file is: Electronics\PCB Components\ESPkamstrup-all-pos-JLCPCB.csv
6. When you press ```Process BOM & CPL```, you will get a warning that the CPL file is missing some data: This is expected, and you can ignore it. The missing parts are the IR LEDs, header pins and D1 Mini. The can be soldered by hand.
7. Check that the components are matched correctly. If not, create a issue on the repository with a description of the problem.
8. In the Component Placements tab, check that all components are placed correctly. The transistors have 3 legs which should line up with the 3 pads on the PCB.
9. Finish the order and wait for the PCBs to arrive.
10. Solder the missing components by hand.