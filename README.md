# RASynBoard-HUB
![Title](/assets/images/RASynBoard_RGB.jpg)

Welcome to the information hub for the Avnet RASynBoard.  RASynBoard is a low-cost evaluation kit that includes the RASynBoard core module with an I/O board for prototyping and development.  Develop your custom ML solution using the evaluation kit, then use the core board SOM in your production hardware design. 

<p align="center">
    RASynBoard EVK<br />
    <img src=./assets/images/1Q5A7940.png width="350">
<br />

[Avnet RASynBoard Buy Link](http://avnet.me/RASynBoard)

## Table of Contents
- [About the RASynBoard](#what-is-the-avnet-rasynboard)
- [RASynBoard GitHub Repositories](#related-repositories)
- [RASynBoard Blogs/Hackster.io Projects](#hacksterio-projects)
- [RASynBoard Online support](#on-line-support)
- [RASynBoard HW documentation](#hardware-documentation)
- [Hands-on self-paced Labs](#self-paced-learning-labs)
- [RASynBoard Accessories](#rasynboard-accessories)
- [RASynBoard 3D Models](#3d-models)
- [Wireless Certification Docs](#wireless-certification-documents)

## What is the Avnet RASynBoard?

### Core Board

The RASynBoard core-board is a tiny (25mm x 30mm), ultra-low power, edge AI/ML board, based on the [Syntiant NDP120 Neural Decision Processor](https://static1.squarespace.com/static/6488b0b8150a045d2d112999/t/650b29219d8c3f0e27f4651e/1695230242406/Syntiant-Product_Brief_NDP120.pdf), [Renesas RA6M4 host MCU](https://www.renesas.com/us/en/products/microcontrollers-microprocessors/ra-cortex-m-mcus/ra6m4-200mhz-arm-cortex-m33-trustzone-high-integration-ethernet-and-octaspi) plus a power-efficient [DA16600 Wi-Fi/BT combo module](https://www.renesas.com/us/en/products/wireless-connectivity/wi-fi/low-power-wi-fi/da16600mod-devkt-da16600-ultra-low-power-wi-fi-bluetooth-low-energy-modules-development-kit?gclid=Cj0KCQiA1rSsBhDHARIsANB4EJZZfMBQ78WT_H04O7F6YbVkDsJeJsSa1Gk6BsGpRPkFix62wG9MFskaAqJREALw_wcB). The NDP120 subsystem includes an onboard [TDK MMICT5838](https://invensense.tdk.com/products/digital/t5838/) digital microphone, 6-axis [TDK ICM42670-P](https://invensense.tdk.com/products/motion-tracking/6-axis/icm-42670-p/) IMU motion sensor and SPI Flash memory.  By including the sensors as part of the NDP120 subsystem, the solution achieves highly efficient processing of acoustic and motion events. Battery and USB-C device connectors facilitate stand-alone use, while a compact under-board connector enables integration with custom OEM boards and additional sensors.

<p align="center">
    Core Board<br />
    <img src=./assets/images/coreBoard.jpg>
<br />

### I/O Board

The IO board (50mm x 30mm) is included for implementation of a compact two board evaluation kit assembly. The I/O board pins-out a subset of the NDP120 and RA6M4 I/Os to popular Pmod, Click header and expansion header footprints; enabling connections to additional external microphones and sensor options. An onboard debugger MCU (SWD and UART interfaces), button switches, RGB LED and removable MicroSD storage, further maximize prototyping versatility and utility.

<p align="center">
    I/O Board<br />
    <img src=./assets/images/IOBoard.jpg>
<br />

## Related Repositories

| Project | Description |
| -- | -- |
| [RASynBoard Out of Box Demo](https://github.com/Avnet/RASynBoard-Out-of-Box-Demo) | Example application intended as a starting point for custom applications.  The repo includes **extensive documentation**, tested releases, feature configuration using a configuration file, and supports Avnet's IoTConnect on AWS and AWS IoT Core cloud connectivity options.  The repo is actively maintained and continually enhanced with additional feature development.  Additionally, the application can be used for custom ML model development and testing using ML models generated on [Edge Impulse Studio](https://edgeimpulse.com/).  This repo also includes a video series to help the user get started and leverage the repo. |
| [RASynBoard Out of Box Demo V1.4.0 W/Temperature and Humidity Sensor](https://github.com/Avnet/RASynBoard-Out-of-Box-Demo/tree/AddTempHumiditySensor) | Example application with additional support for a Renesas HS300X Temperature and Humidity sensor.  See the [Hackster blog](https://www.hackster.io/bwilless/add-a-temperature-humidity-sensor-to-the-avnet-rasynboard-73ce25) for details on this example implementation.|
| [RASynBoard Pump Analytics Demo](https://github.com/Avnet/RASynBoard-Out-of-Box-Demo/tree/pump_analytics) | Example application based on the RASynBoard OOB application that implements a ML model to track pump performance using the built in digital microphone.  See the [Hackster blog](https://www.hackster.io/monica/build-a-dashboard-in-iotconnect-to-monitor-pump-status-e62ed2) for additional details. |
| [RASynBoard Python Demo UI](https://github.com/Avnet/Rasynboard_ew23_demo_GUI_qt) | Python application developed for trade show demos.  Watch the [demo video](http://avnet.me/RASynBoard-OOB-Demo) for more details. The repo includes a windows executable that allows the user to run the demo without having to install any Python dependencies |

## Related Blogs 
### Hackster.io projects
[Search hackster.io for all RASynBoard projects](https://www.hackster.io/search?q="RASynBoard"&i=projects)

| Topic | Description | Difficulty |
| -- | -- | -- |
| [Monitor Pump Status with RASynBoard](https://www.hackster.io/monica/monitor-pump-status-with-rasynboard-311ad1) | Predict pump clogs and failures using the RASynBoard's built-in microphone + Edge Impulse | Intermediate |
| [Build a dashboard in IoTConnect to monitor pump status](https://www.hackster.io/monica/build-a-dashboard-in-iotconnect-to-monitor-pump-status-e62ed2) | This project shows how to create a cloud dashboard to monitor pump analytics over time | Intermediate |
| [Add a Temperature/Humidity Sensor to the Avnet RASynBoard](https://www.hackster.io/bwilless/add-a-temperature-humidity-sensor-to-the-avnet-rasynboard-73ce25) | Extend the number of use cases of the RASynBoard by adding additional sensors | Beginner |
| [Prototyping Predictive Maintenance with RASynBoard](https://www.edgeimpulse.com/blog/pump-up-the-predictions) | Edge Impulse blog reviews how to apply ML to predictive maintenance deployments | Beginner |
| [Determining Compressor State with Audio Classification](https://docs.edgeimpulse.com/experts/audio-projects/compressor-audio-classification-rasynboard) | Edge Impulse blog entry that details how to build an audio classification model to detect pump performance | Intermediate |
| [The RASynPuck Demo, what can you build with the RASynBoard?](https://www.hackster.io/bwilless/the-rasynpuck-demo-what-can-you-build-with-the-rasynboard-bfd912) | Blog shows an example of customizing the RASynBoard Out-of-Box application | Intermediate |

## Hardware Documentation
### Product Brief
[Product Brief](http://avnet.me/rasynboard-pb)
- Includes block diagrams

### User Guide
[Development Guide](http://avnet.me/rasynboard-ug)
- Includes details on all the hardware interfaces and how they pin out to the RA6M4 and NDP120

## On-Line Support

If you require support for the RASynBoard, please post your questions on the [RASynBoard on-line support forum](http://avnet.me/rasynboard-forum).

## Self-Paced Learning Labs

| Title/Link | Description |
| -- | -- |
| [Lab 0](http://avnet.me/ML-WorkshopV2-Lab0) | Details on installing the tools and signing up for free accounts required to complete the self paced learning labs |
| [Lab 1](http://avnet.me/ML-WorkshopV2-Lab1) | Capture training data from the RASynBoard, review the ML model development process in Edge Impulse.  Deploy the Edge Impulse model on your RASynBoard. |
| [Lab 2](http://avnet.me/ML-WorkshopV2-Lab2) | Exercise the Avnet RASynBoard Out of Box example application |

## RASynBoard Accessories

- [Lithium Ion Batteries to power the core board](https://tinycircuits.com/collections/lipos)
- [3D Printable Enclosures](http://avnet.me/RASynEnclosures)

<p align="center">
<br />
    <img src=./assets/images/Enclosures.jpg>
<br />

## 3D models

[3D model files](https://avtinc.sharepoint.com/:f:/t/ET-Downloads/Eq0yaCf3sjJEn-7C-sRmM_EBJKEgCCePUA3-fe5v_bKpRw?e=U4FyXB)

## Wireless Certification Documents

[RASynBoard Certification Documents](https://avtinc.sharepoint.com/:f:/t/ET-Downloads/ErrZqtdTMqtDr3pPJW7dJ-oBj3NIRo1yAmIChJJjOQynzw?e=b4ZjSV)

