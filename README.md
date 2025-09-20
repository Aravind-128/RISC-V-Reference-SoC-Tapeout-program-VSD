# RISC-V-Reference-SoC-Tapeout-program-VSD

 -VSD program end goal is to make a chip that can run applications


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
 
 
