
[![Issues](https://img.shields.io/github/issues/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![Forks](https://img.shields.io/github/forks/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![Stars](https://img.shields.io/github/stars/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/actions)
[![License](https://img.shields.io/github/license/maitesam/OpenADSP)](https://github.com/maitesam/OpenADSP/blob/main/LICENSE)

<p align="center">
  <img width="1100" src="Readme Docs/banner.png" alt="Material Bread logo">
</p>



> An Embedded solution for Digital Signal Processing Applications in Audio signal processing.


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

### Contributions

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



## File Tree

```
.
├── Datasheets
│   ├── AP2112-3.3V.pdf
│   ├── nRF24L01.pdf
│   ├── Readme.md
│   ├── SRV05-4-D.PDF
│   ├── stm32l432kb.pdf
│   └── tlv320aic3100 codec.pdf
├── Documents
│   ├── Code_Print.pdf
│   ├── ibom.html
│   ├── OpenADSP_BLD.jpg
│   ├── OpenADSP_BLD.png
│   ├── PCB Layers
│   │   ├── Audio_Processing_HW_V1.0-B_Adhesive.svg
│   │   ├── Audio_Processing_HW_V1.0-B_Cu.svg
│   │   ├── Audio_Processing_HW_V1.0-B_Mask.svg
│   │   ├── Audio_Processing_HW_V1.0-B_Paste.svg
│   │   ├── Audio_Processing_HW_V1.0-B_Silkscreen.svg
│   │   ├── Audio_Processing_HW_V1.0-Edge_Cuts.svg
│   │   ├── Audio_Processing_HW_V1.0-F_Adhesive.svg
│   │   ├── Audio_Processing_HW_V1.0-F_Cu.svg
│   │   ├── Audio_Processing_HW_V1.0-F_Mask.svg
│   │   ├── Audio_Processing_HW_V1.0-F_Paste.svg
│   │   └── Audio_Processing_HW_V1.0-F_Silkscreen.svg
│   ├── PCB_LayerWise_Export.pdf
│   └── Schematic_OpenADSP.pdf
├── Firmware
│   ├── OpenADSP Debug.launch
│   ├── OpenADSP.ioc
│   ├── Readme.md
│   ├── STM32L432KBUX_FLASH.ld
│   └── temp.html
├── Hardware
│   ├── Analog Filters.kicad_sch
│   ├── Audio_Processing_HW_V1.0.kicad_pcb
│   ├── Audio_Processing_HW_V1.0.kicad_pro
│   ├── Audio_Processing_HW_V1.0.kicad_sch
│   ├── MCU.kicad_sch
│   ├── Power & USB.kicad_sch
│   ├── Readme.md
│   ├── STM32 MCU.kicad_sch
│   ├── untitled.kicad_sch
│   ├── USB&POWER.kicad_sch
│   └── Wireless Tranceiver.kicad_sch
├── Images
│   ├── Bottom_Flat.png
│   ├── Side_Front_view.jpg
│   └── Top_Flat.png
├── LICENSE
├── Mechanical_Files
│   ├── Audio_Processing_HW_V1.0.step
│   ├── Audio_Processing_HW_V1.0.wrl
│   └── readme.txt
├── Readme Docs
│   ├── banner.png
│   ├── ezgif.com-gif-maker.gif
│   ├── icon-5974829_1280.png
│   ├── OpenADSP BOM and 6 more pages - Personal - Microsoft​ Edge 2022-03-02 17-06-42_Trim.mp4
│   ├── OpenADSP.jpg
│   ├── OpenADSP.png
│   └── sound-1837425_1280.png
├── README.md
└── Reference Files
    ├── an4157-stm32f3discovery-peripheral-firmware-examples-stmicroelectronics.pdf
    ├── Deleteme.html
    ├── en.MB1035-F303C-C01_Schematic.pdf
    ├── en.MB1035-F303C-D01_Schematic.pdf
    └── en.MB1035-F303C-E02_Schematic.pdf

9 directories, 59 files

```
## License

This Project is designed under General Public License V3.0 See `LICENSE.txt` for more information.
> https://www.gnu.org/licenses/quick-guide-gplv3.html

<p align="right">(<a href="#top">back to top</a>)</p>



* [Jump To Start](https://github.com/maitesam/OpenADSP/blob/main/README.md#Description)



