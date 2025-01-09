# Project Logs

| Date        | Log |
| ----------- | ----------- |
| 7/1/2025    | Initalized repo and dependencies & ordered all the sensors       |
| 8/1/2025    | Created the block design in Vivado to ultimately set up FreeRTOS in Vitis
- Connected the PL with the Zynq PS via the AXI, and added a GPIO IP Block to the PL also via AXI 
- Vivado neatly generates Verilog code from the block design, which gets synthesized and implemented
- Before generating the bitstream, I assigned the GPIO blocks to the PMOD connectors using XDC constraints, to read the sensor data
- Generated the bitstream file and exported the HW's configuration to Vitis (as an XSA file) for FreeRTOS to run on top of
- TODO: Will need to add SPI or CAN IP blocks and re-generate the XSA file to achieve low-latency comms with future parts in the project         
![image](https://github.com/user-attachments/assets/be97235a-b5ff-4f5b-a520-f1850c1d4cea) |