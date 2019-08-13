Simulation in NGSPICE with schematic from gschem:
=================================================

1.  Open gschem save the file and label the schematic with "sunny_library_components.sub" file by including "spice-include-1.sym" from components.

2.  Take components from library and make the circuit. include "generic-power.sym" to label nodes and "gnd-1.sym" for reference node.

3.  Name the components (prefix "x" the symbols for which subcircuit would be made). Assign values as per the ngspice manual. Save the file.

4.  Make a <same name>.cir and write control statements for simulation (ch15-ngspice manual). also write ".inclide <file name>.net".

5.  Open/create "sunny_library_components.sub" and write the models of the device (prefix-"x"). (to take into account the nonidealities). Save it.


Running ngapice:
6.  Run "gnetlist -g spice-sdb -o <file name>.net <file name>.sch". To generate netlist
7.  Call "ngspice <file name>.cir
8.  Type "run"
9.  Use "plot <node name>" to plot current and voltages.


Running ngspice to get plots:
10. Run "qsim <file name>". To get help type "qsim -help"
    {"ngsim" to generate .cir file too}
11. Plot following the instruction given. You can save the plot too
