# Terasic DE0-CV FPGA Board

DE0-CV User Manual: https://www.intel.com/content/dam/altera-www/global/en_US/portal/dsn/42/doc-us-dsnbk-42-1504012210-de0-cv-user-manual.pdf

DE0-Nano FPGA and VHDL beginner tutorial https://compectroner.wordpress.com/2016/07/14/first-blog-postde0-nano-fpga-and-vhdl-beginner-tutorial/

## 1. Download and install the Intel Quartus Prime Lite Edition on Windows

Intel Quartus Prime Lite Edition https://www.intel.com/content/www/us/en/software/programmable/quartus-prime/download.html

## 2. Create a New Project > Next

* Name the project "Full_Adder" > Next > Finish

* File > New > VHDL File > OK

* Copy and paste adder.vhdl

* Click the arrow to compile

## 3. File > New > University Program VWF (Vector Waveform File)

* Right click the space under "Name" > Insert Node or Bus > Node Finder

* Click "List" then ">>" > OK > OK

  Right click "i0" > Click the Symbol for Random Values > Every grid interval > OK

  Right click "i1" > Click the Symbol for Random Values > Every grid interval > OK

  Right click "ci" > Click the Symbol for Random Values > Every grid interval > OK

* Simulation > Generate ModelSim Testbench and Script

## 4. Program FPGA board

DE0-CV User Manual, Pages 24 to 25: https://www.intel.com/content/dam/altera-www/global/en_US/portal/dsn/42/doc-us-dsnbk-42-1504012210-de0-cv-user-manual.pdf

* Assignment > Device > Cyclone V E > 5CEBA4F23C7

* Assignment > Pin Planner

  i0 > PIN_U7 -- KEY0

  i1 > PIN_W9 -- KEY1

  ci > PIN_M7 -- KEY2

  co > PIN_AA1 -- LEDR1
  
  s > PIN_AA2 -- LEDR0
  
* Double-click the blue arrows under Compilation one at a time

## 5. Tool > Programmer > Hardware Setup > USB Blaster > Start
