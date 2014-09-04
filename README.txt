THIS IS MY README!

Intro:
  The f0_template is meant to help users get started quickly on the F0 Discovery 
  Board from ST Micro, using Open Source Tools.

Tools:
  1. Eclipse Luna
  2. Open OCD
  3. ST Link V2
  4. GNU ARM Toolchain

General Notes:
  Currently this is only configured for Windows machines. Although OSX and 
  Ubuntu/Debian Linux Flavors have been integrated, they do not yet exist in 
  this template. 

  Project Template is for Eclipse Luna only. Have not checked for any backwords 
  compatibility.

  The concept is to export this template from Git, and change to the appropriate
  project name. When this is done, you will need to change the include
  directories at C/C++ General->Paths and Symbols in the Project Properties
  dialogue. 

Windows Notes:
  Windows users will need to install a make and telnet utility. My easiest way
  to integrate these two items is by installing Cygwin and the appropriate 
  packages. This is easily understood how by googling.

  Windows users will need to download and install the ST-Link V2 Drivers.
    - Download: http://www.st.com/web/en/catalog/tools/PF258167
    
  Windows users will need to download and install Open OCD.

    - Download Location: http://sourceforge.net/projects/openocd/
    - Install Location: C:\openocd-0.8.0
    - Create an external tool configuration (eclipse feature) that will launch 
      Open OCD. Will need to add the following line to the arguements:
        -f board/stm32f0discovery.cfg
    - No working directory is needed to launch Open OCD.

  Windows users will need to install the GNU ARM Tool Chain.
    - Download Location: https://launchpad.net/gcc-arm-embedded/4.8/4.8-2014-q2-update/+download/gcc-arm-none-eabi-4_8-2014q2-20140609-win32.exe
        - This is the minimal build that will work. Choose the appropriate 
          32/64 bit version of OS that you are using.
    - Should install at location: C:\Program Files (x86)\GNU Tools ARM Embedded\4.8 2014q2
        - This matters, or you will have to change the current GDB configurations.

    


