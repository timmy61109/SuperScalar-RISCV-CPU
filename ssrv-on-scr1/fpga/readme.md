* fpga/

    The FPGA demonstration project is based on Altera DE2-115 development board. 

    * DE2-115/ 
    
    The main directory of this FPGA project. Open " DE2_115.qsf" file to find more details. DE2-115.v is the top module.

    * pll/
    
    A PLL ip generated by "MegaWizard Plug-In Manager", which will turn a 50 MHz clock to a 30 MHz clock.
    
    * ram/
    
    A 64KB dual-port ram generated by "MegaWizard Plug-In Manager", which contains a mif file: code.mif. This mif file is converted from build/ dhrystone21_imc_noinline.hex.

    * rtl/ --- The SSRV CPU core.

    * scr1/ --- SCR1 source files.

    * test/

    Two synthesizable files: rxtx.v, which is a simple UART verilog file; and "ssrv_memory.v, which instantiates the 64KB dualport ram.
    
    The FPGA board should be connected with a UART terminal, which has a configuration of 9600, even, 1 stop bit. You can change the baud rate through the parameters of rxtx.v. Please open DE2-115.v, find the instantiation of rxtx and give your "mhz" and "baud".

 
