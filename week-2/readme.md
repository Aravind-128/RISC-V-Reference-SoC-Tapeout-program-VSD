 # 1. What is a System on a chip(SoC) ?
  A **System on a Chip (SoC)** is a complete computer system built on a single chip, integrating multiple components such as CPU,
  GPU, memory, and I/O ports. It is widely used in compact, power-efficient devices like smartphones, tablets, smartwatches,
  and IoT gadgets.

 # Main components 
 
   - **CPU**: Performs main processing and control tasks.
   - **Memory**: Includes RAM for temporary data and Flash/ROM for permanent storage.
   - **I/O Ports**: Enable communication with external devices (USB, camera, etc.).
   - **GPU**: Handles graphics and visuals.
   - **DSP**: Processes audio/video signals efficiently.
   - **Power Management Unit**: Controls energy usage to extend battery life.
   - **Special Features**: Wi-Fi, Bluetooth, and security modules depending on device type.
     
 # Advantages

   - **Compact**: Saves space by combining all components in one chip.
   - **Power Efficient**: Consumes less energy—ideal for portable devices.
   - **High Performance**: Faster data communication within the chip.
   - **Cost Effective**: Cheaper and simpler manufacturing.
   - **Reliable**: Fewer parts mean fewer chances of hardware failure.

 # Applications
   - Used in mobile devices, wearables, IoT devices, smart TVs, vehicles, and appliances.

 # Popular SoCs
   - Apple A-Series, Qualcomm Snapdragon, Samsung Exynos, NVIDIA Tegra.

 # Challenges with SoCs
   - **Complex Design**: Integrating multiple systems on one chip is difficult.
   - **Heat Management**: High component density can cause overheating.
   - **Limited Flexibility**: Hard to modify once manufactured.

# 2.Types of SoCs
  - **Microcontroller-based SoCs**: Designed for simple control tasks with low power use, ideal for home appliances, cars, and IoT devices.
  - **Microprocessor-based SoCs**: Built for complex, multitasking applications that require high processing power, such as smartphones and tablets.
  - **Application-Specific SoCs**: Custom-built for specialized, high-performance tasks like graphics, AI, or networking, optimized for speed and efficiency in  specific functions.

 # SoC design flow

 ![My logo](soc_design_floe)

 # 3.Introduction to VSDBabySoC

  **VSDBabySoC**is a compact RISC-V-based System on Chip (SoC) designed for testing multiple open-source IP cores and  
  calibrating analog components. It integrates:
   - **RVMYTH CPU**: Handles digital data processing.
   - **Phase-Locked Loop (PLL)**: Generates a stable clock signal to synchronize all components.
   - **10-bit Digital-to-Analog Converter (DAC)**: Converts digital data into analog signals for external devices like  TVs or mobile phones.

 # 1.Initialization & Clock Generation:
   - The PLL activates upon input, producing a synchronized clock to coordinate CPU and DAC operations.
   - Ensures data integrity and timing accuracy.

 # Data Processing (RVMYTH CPU):
   - Uses its registers (e.g., r17) to cycle through digital values for the DAC.
   - Generates continuous digital streams for analog conversion.

 # Analog Signal Generation (DAC):
   - Converts digital values from RVMYTH into analog outputs.
   - Interfaces with consumer electronics to produce sound or video.

 
 
 
