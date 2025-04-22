jtagconfig --setparam 1 JtagClock 16M 

quartus_pgm -c 1 -m jtag -o "pvi;agilex_flash_image.hps.jic"
