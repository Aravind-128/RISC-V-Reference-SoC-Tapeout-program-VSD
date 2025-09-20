# RISC-V-Reference-SoC-Tapeout-program-VSD

   - **VSD program end goal is to make a chip that can run applications**
   - **The chip supports a frequency range from 100 MHz up to 130 MHz**
   - **DESIGN FLOW**
    -` RTL DESIGN ->  SYNTHESIS  -> RTL2GDS -> PHYSICAL DESIGN -> DRC/LVS checks -> CHIP `

---

- **Step 1:** We take the testbench and compile it with GCC, producing an output **O0**.  
- **Step 2:** According to the specifications, the C model generates the output **O1**.  
- **Step 3:** A Register-Transfer Level (RTL) implementation in Verilog provides the soft copy of the hardware, which integrates the processor and peripherals within a typical SoC design flow, producing output **O2**.  
- **Step 4:** SoC integration of GPIOs is carried out as part of the RTL-to-GDSII flow, producing output **O3**.  
- **Step 5:** Post-GDSII, Design Rule Checking (DRC) and Layout Versus Schematic (LVS) checks are conducted to validate the physical layout.  
- **Step 6:** Upon completion of design and testing, the chip generates output **O4**, which was found to be equal to **O1**, **O2**, and **O3**.
    
---

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
 
 
