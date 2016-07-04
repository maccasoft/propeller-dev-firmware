## Propeller Development Board

![The Board](board.jpg)

This is my own version of a [Parallax Propeller](https://www.parallax.com) development board.

Uses a PIC microcontroller for the USB-Serial interface, can be powered from either USB or a dedicated power source, includes
an EEPROM to store the program and data, and provides a 2x20 pin header exposing all 32 I/O pins from the Propeller microcontroller,
power and control lines.

Compatible with all standard Propeller development tools.

**Parts List**

* R1 = 4.700 ohm 1/4 watt  
* R2 = 4.700 ohm 1/4 watt  
* R3 = 220 ohm 1/4 watt  
* R4 = 220 ohm 1/4 watt  
* R5 = 220 ohm 1/4 watt  
* R6 = 33.000 ohm 1/4 watt  
* C1 = 100.000 pF poli  
* C2 = 100.000 pF poli  
* C3 = 100.000 pF poli  
* C4 = 10 uF 63v elettr.  
* C5 = 10 uF 63v elettr.  
* C6 = 100.000 pF poli  
* C7 = 27 pF disc  
* C8 = 27 pF disc  
* C9 = 10.000 pF poli  
* DL1 = Red LED  
* DL2 = Yellow LED  
* DL3 = Green LED  
* XTAL1 = 5 MHz crystal  
* XTAL2 = 12 MHz crystal  
* IC1 = P8X32A  
* IC2 = 24LC512  
* IC3 = PIC18F14K50  
* IC4 = LM1117T-3.3  
* TR1 = Transistor NPN BC547  
* CN1 = USB-B connector  
* CN2 = 2.1mm DC power connector  
* CN3 = 2x20 pin header  
* JP1 = 1x3 pin header  
* P1 =  Button  

**JP1**

Power source selection:

```
+-+  
|1| USB  
|2| VIN  
|3| EXT  
+-+  
```

short pins 1-2 to power from USB  
short pins 2-3 to power from external source.

**CN3**

From top, P0/P1 are near the PIC/USB microcontroller.

```
+-------+-------+  
|     P0|P1     |  
|     P2|P3     |  
|     P4|P5     |  
|     P6|P7     |  
|     P8|P9     |  
|    P10|P11    |  
|    P12|P13    |  
|    P14|P15    |  
|    P16|P17    |  
|    P18|P19    |  
|    P20|P21    |  
|    P22|P23    |  
|    P24|P25    |  
|    P26|P27    |  
|SDA/P29|N.C.   |  
|SCL/P28|XI     |  
| TX/P30|RTS    |  
| RX/P31|CTS    |  
|  RESET|+3.3v  |  
|    GND|VIN    |  
+-------+-------+  
```

PCBs are shared on [OSH Park](https://oshpark.com) and can be ordered from there:
[https://oshpark.com/shared_projects/KALqBSpm](https://oshpark.com/shared_projects/KALqBSpm)
