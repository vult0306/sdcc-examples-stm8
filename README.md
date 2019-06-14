stm8-examples-sdcc
==================

Related software:

http://sdcc.sourceforge.net/
https://github.com/vdudouyt/stm8flash

Install stlink
    sudo apt-get update
    sudo apt-get install cmake
    sudo apt-get install libusb-1.0-0-dev
    git clone https://github.com/texane/stlink stlink
    cd stlink
    make
    sudo udevadm control --reload
    Reboot
    
Install compiler
    sudo apt-get install sdcc

Install stm8s flash tool
    git clone https://github.com/vdudouyt/stm8flash.git
    cd stm8flash
    make
    sudo make install
    
Install example project
    git clone https://github.com/vdudouyt/sdcc-examples-stm8.git
    cd sdcc-examples-stm8
    
flash command
    stm8flash -c stlinkv2 -p stm8s103 -w blinky.ihx
