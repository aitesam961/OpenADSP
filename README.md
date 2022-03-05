
[![Issues](https://img.shields.io/github/issues/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![Forks](https://img.shields.io/github/forks/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![Stars](https://img.shields.io/github/stars/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![License](https://img.shields.io/github/license/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/blob/main/LICENSE)

<p align="center">
  <img width="1100" src="Readme Docs/banner.png" alt="Material Bread logo">
</p>


> An Embedded solution for Digital Signal Processing Applications in Audio Domain. 

## Table of contents
* [Description](https://github.com/maitesam/OpenADSP/blob/main/README.md#Description)
* [Block Diagram](https://github.com/maitesam/OpenADSP/blob/main/README.md#block-diagram)
* [Working Explained](https://github.com/maitesam/OpenADSP/blob/main/README.md#Working-Explained)
* [Ordering Boards](https://github.com/maitesam/OpenADSP/blob/main/README.md#Ordering-Boards)
* [Assembly](https://github.com/maitesam/OpenADSP/blob/main/README.md#Assembly)
* [Flashing Firmware](https://github.com/maitesam/OpenADSP/blob/main/README.md#Flashing-Firmware)
* [Contribution](https://github.com/maitesam/OpenADSP/blob/main/README.md#Contribution)
* [License](https://github.com/maitesam/OpenADSP/blob/main/README.md#License)


## Description
This device is designed to Take data from Microphone and Process it. Later it could be sent to a wirelessly connected devices Over Bluetooth.
Aside from this, the device can stream data to host computer over USB interface.

The PCB embedds a STM32L432 MCU which is extremely capable of handling Demanding tasks such as Digital Signal Processing.
The DSP scripts could be implemented in the firmware.

## Preview
<p align="center">
  <img width="400" src="Images\Top_Flat.png">
  <img width="400" src="Images\Bottom_Flat.png" alt="Material Bread logo">
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
[Check Out PCBWay](https://www.pcbway.com/setinvite.aspx?inviteid=440401)

Note: I am not affiliated with PCBWay. However, I just like their service and build quality.


## Assembly Guide
Please Refer to [Hardware Readme](https://github.com/maitesam/OpenADSP/blob/main/Hardware) for Assembly Instructions.

## Flashing Firmware
Please Refer to [Firmware Readme](https://github.com/maitesam/OpenADSP/tree/main/Firmware) to find more details about Flashing FIrmware.

## Contributions

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Roadmap
* [x] Concept Proof
* [x] Research & Information
* [x] Finalizing The Idea
* [x] Schematics
* [x] PCB Design
* [ ] Firmware Development
* [ ] Validation & Testing
* [ ] Documentation
* [ ] Future Improvements





## License

This Project is designed under General Public License V3.0 See `LICENSE.txt` for more information.
> https://www.gnu.org/licenses/quick-guide-gplv3.html

<p align="right">(<a href="#top">back to top</a>)</p>



* [Jump To Start](https://github.com/maitesam/OpenADSP/blob/main/README.md#Description)



