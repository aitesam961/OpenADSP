<p align="center">
  <img width="1100" src="Readme Docs/banner.png" alt="Material Bread logo">
</p>

### !!! Caution:Readme Under Progress.......

> An Embedded Digital Signal Processing Device for Audio signals.

## Table of contents
* [Description](##Description)
* [Block Diagram](##Block-Diagram)
* [Working Explained](##Working-Explained)
* [Ordering Boards](##Ordering-Boards)
* [Assembly](##Assembly)
* [Flashing Firmware](##Flashing-Firmware)
* [Contribution](##Contribution)
* [License](##License)


## Description
This device is designed to Take data from Microphone and Process it. Later it could be sent to a wirelessly connected devices Over Bluetooth.
Aside from this, the device can stream data to host computer over USB interface.

The PCB embedds a STM32L432 MCU which is extremely capable of handling Demanding tasks such as Digital Signal Processing.
The DSP scripts could be implemented in the firmware.

## Preview
<p align="center">
  <img width="600" src="Images\Top_Flat.png">
  <img width="600" src="Images\Bottom_Flat.png" alt="Material Bread logo">
</p>

## Block Diagram
The Block Diagram Illustrates the connectivity inside The Board.
<p align="center">
  <img width="600" src="Documents\OpenADSP_BLD.jpg">
</p>

## Working Explained
This device is Designed for Digital Signal Processing applications.
The idea is to take Audio Data from a microphone, process it & Transmit to client devices.
#### What Type of Processing?
It features an STM32L432 Microcontroller with an ARM Cortex M4F (aka Black Pill). The device can be programmed to Apply Digital Filters and Effects on the audio data.
The very basic example is a Low Pass & High Pass filters.
The Incoming Audio Signal is converted to Digital (By ADC) and then Passed to STM32 which Applies programmed filters.


### Connectivity
The device is loaded with Two modes of communication.

* Bluetooth (2.4GHz)
* USB 2.0

The device is capable of Reading Data, applying filters and then Sending it wirelessly over to a Bluetooth Client
OR 
It Can be used as a USB OTG host device to send data stream over USB 2.0 Interface.

## Ordering Boards
You Can manufacture the PCBs from PCBWay.

### Placing Order at PCBWay

## Assembly Guide
## Flashing Firmware
## Contribution
## License



- Badges 
- Logo
- Gif
- Installation 
- User Guide
- Additional
- Contribution
- License



## Coming Soon........


* [Jump To Start](#Back-To-Top)



