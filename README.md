# RISC-V-Reference-SoC-Tapeout-program-VSD

   ** VSD program end goal is to make a chip that can run applications **
   ** The chip supports a frequency range from 100 MHz up to 130 MHz **
   **  RTL DESIGN ->  SYNTHESIS  -> RTL2GDS -> PHYSICAL DESIGN -> DRC/LVS checks -> CHIP  **

 step -1.we take the testbench and compile it with GCC , produce a output O0.
 step -2.According to the specifications, the C model generates the output O1.
 step -3.A Register-Transfer Level (RTL) implementation in Verilog provides the soft copy of the hardware, which                  integrates the processor and peripherals within a typical SoC design flow, produce a output O2.
 step -4.SoC integration of GPIOs is carried out as part of the RTL-to-GDSII flow , produce a output O3.
 step -5.Post-GDSII, Design Rule Checking (DRC) and Layout Versus Schematic (LVS) checks are conducted to validate the            physical layout.
 step -6.Upon completion of design and testing, the chip generated output O4, which was found to be equal 
         to O1, O2, and O3.
    


 # Week- 0 - Installation of tools 

  System requirements
     -6GB RAM, 50 GB HDD
     -Ubuntu 20.04+
     -4vCPU
     

  # Yosys 
     $ sudo apt-get update
     $ git clone https://github.com/YosysHQ/yosys.git
     $ cd yosys
     $ sudo apt install make (If make is not installed please install it)
     $ sudo apt-get install build-essential clang bison flex \
     libreadline-dev gawk tcl-dev libffi-dev git \
     graphviz xdot pkg-config python3 libboost-system-dev \
     libboost-python-dev libboost-filesystem-dev zlib1g-dev
     $ make config-gcc
    $ make
    $ sudo make install
   

  # iverilog
    sudo apt-get update
    sudo apt-get install iverilog

  # Gtkwave 
    sudo apt-get update
    sudo apt install gtkwave
 
 
