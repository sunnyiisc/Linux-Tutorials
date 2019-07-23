Vivado Installation:
====================

Before Installation steps:
--------------------------
Linking Library else the installtion will get struck at final processing..

Step-1:
    sudo ln -s /lib64/libtinfo.so.6 /lib64/libtinfo.so.5
    // linking .5 file with .6

Step-2:
    sudo dnf install libpng12
    // library for DocNav which is not pre installed in fedora

Step-3:
    Run the xsetup (./xsetup) or the .bin file 
    for running .bin file : 
        chmod +x <.bin file>
        ./<.bin file>
        
Running Vivado:
---------------
Step-1:
    Goto the installed directory (eg- cd /opt/Xilinx/Vivado/2015.1/)
    //sourcing settings64.sh
        source settings64.sh
    
Step-2:
    Run these commands:
    
        mkdir ~/vivado
        cd ~/vivado
        vivado &

Step-3:
    For installing Driver of FPGA board:
    
        Check that /etc/udev/rules.d/52-xilinx-digilent-usb.rules is installed. If not, run:
        /opt/Xilinx/Vivado/2016.2/data/xicom/cable_drivers/lin64/install_script/install_drivers/install_digilent.sh

