# Arduino core support for STM32 based boards
[![GitHub release](https://img.shields.io/github/release/stm32duino/Arduino_Core_STM32.svg)](https://github.com/stm32duino/Arduino_Core_STM32/releases/latest)
![GitHub All Releases](https://img.shields.io/github/downloads/stm32duino/Arduino_Core_STM32/total.svg?label=downloads%20since%201.4.0)
[![GitHub commits](https://img.shields.io/github/commits-since/stm32duino/Arduino_Core_STM32/1.8.0.svg)](https://github.com/stm32duino/Arduino_Core_STM32/compare/1.8.0...master)
[![Build Status](https://travis-ci.com/stm32duino/Arduino_Core_STM32.svg?branch=master)](https://travis-ci.com/stm32duino/Arduino_Core_STM32)

* [Introduction](https://github.com/stm32duino/Arduino_Core_STM32#Introduction)<br>
* [Getting Started](https://github.com/stm32duino/Arduino_Core_STM32#getting-started)<br>
* [Boards available](https://github.com/stm32duino/Arduino_Core_STM32#boards-available)<br>
* [Troubleshooting](https://github.com/stm32duino/Arduino_Core_STM32#troubleshooting)<br>
* [Wiki](https://github.com/stm32duino/wiki/wiki/)

## Introduction

This repo adds the support of STM32 MCU in Arduino IDE.<br>

This porting is based on:
* [STM32Cube MCU Packages](https://www.st.com/en/embedded-software/stm32cube-mcu-packages.html) including:
    * The HAL hardware abstraction layer, enabling portability between different STM32 devices via standardized API calls
    * The Low-Layer (LL) APIs, a light-weight, optimized, expert oriented set of APIs designed for both performance and runtime efficiency
    * CMSIS device defintion for STM32
* [CMSIS](https://developer.arm.com/embedded/cmsis): Cortex Microcontroller Software Interface Standard (CMSIS) is a vendor-independent hardware abstraction layer for the Cortex®-M processor series and defines generic tool interfaces. It has been packaged as a module for Arduino IDE: https://github.com/stm32duino/ArduinoModule-CMSIS
* [GNU Arm Embedded Toolchain](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm): Arm Embedded GCC compiler, libraries and other GNU tools necessary for bare-metal software development on devices based on the Arm Cortex-M. Packages are provided thanks [The xPack GNU Arm Embedded GCC](https://xpack.github.io/arm-none-eabi-gcc/): https://github.com/xpack-dev-tools/arm-none-eabi-gcc-xpack

## Getting Started

This repo is available as a package usable with [Arduino Boards Manager](https://www.arduino.cc/en/guide/cores).

Use this link in the "*Additional Boards Managers URLs*" field:

https://github.com/stm32duino/BoardManagerFiles/raw/master/STM32/package_stm_index.json


For full instructions on using the "**Boards Manager**", see the [Getting Started](https://github.com/stm32duino/wiki/wiki/Getting-Started) page.

Advanced user can use the repository to benefit from the latest development. See the [Using git repository](https://github.com/stm32duino/wiki/wiki/Using-git-repository) page.

User can add a STM32 based board following this [wiki](https://github.com/stm32duino/wiki/wiki/Add-a-new-variant-(board)).

## Boards available

| Status | [Nucleo 144](https://www.st.com/content/st_com/en/products/evaluation-tools/product-evaluation-tools/mcu-eval-tools/stm32-mcu-eval-tools/stm32-nucleo-boards.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [Nucleo F207ZG](http://www.st.com/en/evaluation-tools/nucleo-f207zg.html) | *0.2.0* |  |
| :green_heart: | [Nucleo F429ZI](http://www.st.com/en/evaluation-tools/nucleo-f429zi.html) | *0.1.0* |  |
| :green_heart: | [Nucleo F767ZI](http://www.st.com/en/evaluation-tools/nucleo-f767zi.html) | *1.4.0* |  |
| :green_heart: | [Nucleo L496ZG](http://www.st.com/en/evaluation-tools/nucleo-l496zg.html) | *1.3.0* |  |
| :green_heart: | [Nucleo L496ZG-P](http://www.st.com/en/evaluation-tools/nucleo-l496zg-p.html) | *1.3.0* |  |
| :green_heart: | [Nucleo L4R5ZI](http://www.st.com/en/evaluation-tools/nucleo-l4r5zi.html) | *1.4.0* |  |
| :green_heart: | [Nucleo L4R5ZI-P](http://www.st.com/en/evaluation-tools/nucleo-l4r5zi-p.html) | *1.4.0* |  |
| :green_heart: | [Nucleo H743ZI(2)](https://www.st.com/en/evaluation-tools/nucleo-h743zi.html) | *1.5.0* | Nucleo H743ZI2 since 1.6.0 |

| Status | [Nucleo 64](https://www.st.com/content/st_com/en/products/evaluation-tools/product-evaluation-tools/mcu-eval-tools/stm32-mcu-eval-tools/stm32-nucleo-boards.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [Nucleo F030R8](http://www.st.com/en/evaluation-tools/nucleo-f030r8.html) | *0.2.0* |  |
| :green_heart: | [Nucleo F091RC](http://www.st.com/en/evaluation-tools/nucleo-f091rc.html) | *0.1.0* |  |
| :green_heart: | [Nucleo F103RB](http://www.st.com/en/evaluation-tools/nucleo-f103rb.html) | *0.2.0* |  |
| :green_heart: | [Nucleo F302R8](http://www.st.com/en/evaluation-tools/nucleo-f302r8.html) | *1.1.0* |  |
| :green_heart: | [Nucleo F303RE](http://www.st.com/en/evaluation-tools/nucleo-f303re.html) | *0.1.0* |  |
| :green_heart: | [Nucleo F401RE](http://www.st.com/en/evaluation-tools/nucleo-f401re.html) | *0.2.1* |  |
| :green_heart: | [Nucleo F411RE](http://www.st.com/en/evaluation-tools/nucleo-f411re.html) | *0.2.1* |  |
| :green_heart: | [Nucleo F446RE](http://www.st.com/en/evaluation-tools/nucleo-f446re.html) | *1.1.1* |  |
| :green_heart: | [Nucleo G071RB](https://www.st.com/en/evaluation-tools/nucleo-g071rb.html) | *1.6.0* |  |
| :green_heart: | [Nucleo G431RB](https://www.st.com/en/evaluation-tools/nucleo-g431rb.html) | *1.7.0* |  |
| :green_heart: | [Nucleo G474RE](https://www.st.com/en/evaluation-tools/nucleo-g474re.html) | *1.7.0* |  |
| :green_heart: | [Nucleo L053R8](http://www.st.com/en/evaluation-tools/nucleo-l053r8.html) | *0.1.0* |  |
| :green_heart: | [Nucleo L073RZ](http://www.st.com/en/evaluation-tools/nucleo-l073rz.html) | *1.4.0* |  |
| :green_heart: | [Nucleo L152RE](http://www.st.com/en/evaluation-tools/nucleo-l152re.html) | *1.0.0* |  |
| :green_heart: | [Nucleo L452RE](http://www.st.com/en/evaluation-tools/nucleo-l452re.html) | *1.5.0* |  |
| :green_heart: | [Nucleo L452RE-P](http://www.st.com/en/evaluation-tools/nucleo-l452re-p.html) | *1.8.0* |  |
| :green_heart: | [Nucleo L476RG](http://www.st.com/en/evaluation-tools/nucleo-l476rg.html) | *0.1.0* |  |
| :green_heart: | [P-Nucleo-WB55RG](https://www.st.com/en/evaluation-tools/p-nucleo-wb55.html) | *1.6.0* | No BLE support |

| Status | [Nucleo 32](https://www.st.com/content/st_com/en/products/evaluation-tools/product-evaluation-tools/mcu-eval-tools/stm32-mcu-eval-tools/stm32-nucleo-boards.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [Nucleo F303K8](http://www.st.com/en/evaluation-tools/nucleo-f303k8.html) | *1.1.0* |  |
| :green_heart: | [Nucleo G431KB](https://www.st.com/en/evaluation-tools/nucleo-g431kb.html) | *1.7.0* |  |
| :green_heart: | [Nucleo L031K6](http://www.st.com/en/evaluation-tools/nucleo-l031k6.html) | *1.1.1* |  |
| :green_heart: | [Nucleo L412KB](http://www.st.com/en/evaluation-tools/nucleo-l412kb.html) | *1.5.0* |  |
| :green_heart: | [Nucleo L432KC](http://www.st.com/en/evaluation-tools/nucleo-l432kc.html) | *0.2.0* |  |

| Status | [Discovery](https://www.st.com/content/st_com/en/products/evaluation-tools/product-evaluation-tools/mcu-eval-tools/stm32-mcu-eval-tools/stm32-discovery-kits.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [32F0308DISCOVERY](http://www.st.com/en/evaluation-tools/32f0308discovery.html) | *1.3.0* |  |
| :green_heart: | [32F072BDISCOVERY](https://www.st.com/en/evaluation-tools/32f072bdiscovery.html) | *1.5.0* |  |
| :green_heart: | [STM32VLDISCOVERY](https://www.st.com/en/evaluation-tools/stm32vldiscovery.html) | 0.2.1 |  |
| :green_heart: | [STM32F407G-DISC1](http://www.st.com/en/evaluation-tools/stm32f4discovery.html) | *0.1.0* |  |
| :green_heart: | [STM32F746G-DISCOVERY](http://www.st.com/en/evaluation-tools/32f746gdiscovery.html) | *0.1.0* |  |
| :yellow_heart: | [STM32G0316-DISCO](https://www.st.com/en/evaluation-tools/stm32g0316-disco.html) | **1.9.0** |  |
| :green_heart: | [B-L072Z-LRWAN1](http://www.st.com/en/evaluation-tools/b-l072z-lrwan1.html) | *1.1.0* |  |
| :green_heart: | [B-L475E-IOT01A](http://www.st.com/en/evaluation-tools/b-l475e-iot01a.html) | *1.0.1* |  |

| Status | [Eval](https://www.st.com/en/evaluation-tools/stm32-eval-boards.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [STEVAL-MKSBOX1V1 (SensorTile.box)](https://www.st.com/en/evaluation-tools/steval-mksbox1v1.html) | *1.7.0* |  |

| Status | [STM32MP1 series coprocessor](https://www.st.com/content/st_com/en/products/microcontrollers-microprocessors/stm32-arm-cortex-mpus/stm32mp1-series.html) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [STM32MP157A-DK1](https://www.st.com/en/evaluation-tools/stm32mp157a-dk1.html) | *1.8.0* | See [the documentation](https://github.com/stm32duino/Arduino_Core_STM32/tree/master/variants/STM32MP157_DK/README.md) to use this board|
| :green_heart: | [STM32MP157C-DK2](https://www.st.com/en/evaluation-tools/stm32mp157c-dk2.html) | *1.8.0* | See [the documentation](https://github.com/stm32duino/Arduino_Core_STM32/tree/master/variants/STM32MP157_DK/README.md) to use this board|


| Status | Generic STM32F0xx | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [STM32F030F4 Demo board](https://stm32-base.org/boards/STM32F030F4P6-STM32F030-DEMO-BOARD-V1.1) | *1.5.0* |  |

| Status | Generic STM32F1xx | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [BluePill F103C(6-8-B)](https://stm32-base.org/boards/STM32F103C8T6-Blue-Pill) | *1.2.0* | USB CDC support since *1.5.0*, Maple bootloaders support since *1.6.0* |
| :green_heart: | [BlackPill F103C(8-B)](https://stm32-base.org/boards/STM32F103C8T6-Black-Pill) | *1.5.0* |  |
| :green_heart: | [Generic F103R(8-B-C-E)T6](https://stm32-base.org/boards/STM32F103RET6-Generic-Board) | *1.7.0* | Blue Button |
| :yellow_heart: | Generic F103Z(C-D-E-F-G) | **1.9.0** |  |
| :green_heart: | HY-TinySTM103T | *1.5.0* |  |
| :green_heart: | MapleMini F103CB | *1.2.0* | USB CDC support since *1.5.0*, Maple bootloaders support since *1.6.0* |
| :yellow_heart: | [Vcc-Gnd F103ZET6](http://www.vcc-gnd.com/rtd/html/STM32/quickref.html#stm32f1) | **1.9.0** | [Standard](https://stm32-base.org/boards/STM32F103ZET6-VCC-GND-XLarge) and Mini |


| Status | Generic STM32F3xx | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [RobotDyn BlackPill F303CC](https://robotdyn.com/catalog/development-boards/stm-boards-and-shields.html) | *1.6.1* |  |

| Status | Generic STM32F4xx | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [Adafruit Feather STM32F405 Express](https://www.adafruit.com/product/4382) | *1.8.0* |  |
| :green_heart: | BlackPill F401CC | *1.7.0* |  |
| :yellow_heart: | BlackPill F411CE | **1.9.0** |  |
| :green_heart: | [Black F407VET6](https://stm32-base.org/boards/STM32F407VET6-STM32-F4VE-V2.0) | *1.4.0* | VG/ZE/ZG in *1.5.0* |
| :green_heart: | [Blue F407VET6 Mini](https://stm32-base.org/boards/STM32F407VET6-VCC-GND-Small) | *1.4.0* |  |
| :green_heart: | Core Board F401RC | *1.7.0* |  |
| :green_heart: | [DIYMORE STM32F407VGT](https://stm32-base.org/boards/STM32F407VGT6-diymore) | *1.5.0* |  |
| :green_heart: | FK407M1 | *1.5.0* |  |
| :yellow_heart: | Generic F401C(B-C-D-E) | **1.9.0** |  |
| :green_heart: | Generic F401R(B-C-D-E) | *1.8.0* |  |
| :yellow_heart: | Generic F410R(8-B) | **1.9.0** |  |
| :yellow_heart: | Generic F411C(C-E) | **1.9.0** |  |
| :yellow_heart: | Generic F411R(C-E) | **1.9.0** |  |
| :yellow_heart: | Generic F446R(C-E) | **1.9.0** |  |

| Status | Generic STM32L0xx | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [PX-HER0](https://piconomix.com/fwlib/_p_i_c_o_n_o_m_i_x__s_t_m32__h_e_r_o__b_o_a_r_d.html) | *1.8.0* |  |
| :green_heart: | [ThunderPack](https://github.com/jgillick/ThunderPack) | *1.8.0* |  |

| Status | 3D printer boards | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [ARMED V1](https://github.com/ktand/Armed) | *1.5.0* |  |
| :green_heart: | [EExtruder F030 V1](https://github.com/ghent360/PrntrBoard/tree/tmc2130-redesign/EExtruder) | *1.5.0* | Small companion board for Prntr Board V1 |
| :green_heart: | [Malyan M200 V1](http://malyansys.com/product/m200-v1/) | *1.5.0* |  |
| :green_heart: | [Malyan M200 V2](http://malyansys.com/product/m200-v2/) | *1.5.0* |  |
| :green_heart: | [Malyan M300](http://malyansys.com/product/m300/) | *1.8.0* |  |
| :green_heart: | [Prntr Board V1](https://github.com/ghent360/PrntrBoard) | *1.5.0* |  |
| :green_heart: | [Prntr Board V2](https://github.com/ghent360/PrntrBoardV2) | *1.8.0* |  |
| :green_heart: | [RemRam v1](https://github.com/hasenbanck/remram) | *1.4.0* |  |
| :green_heart: | [RUMBA32](https://github.com/Aus3D/RUMBA32) | *1.5.0* |  |
| :green_heart: | [STEVAL-3DP001V1](https://www.st.com/en/evaluation-tools/steval-3dp001v1.html) | *1.6.0* |  |
| :green_heart: | [VAkE v1.0](https://www.facebook.com/pages/category/Product-Service/VAkE-Board-2290066274575218/) | *1.6.0* |  |

| Status | LoRa boards | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [RAK811 LoRa Tracker](https://www.rakwireless.com/en/) | *1.4.0* | [Wiki](https://github.com/stm32duino/wiki/wiki/Connectivities#lora) |
| :green_heart: | [RHF76-052](https://www.ai-thinker.com/) | *1.7.0* | Basic support |

| Status | Electronic Speed Controller boards | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | Wraith V1 ESC | *1.8.0* |  |

| Status | Generic flight controllers | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | Afro Flight Rev5 (8/12MHz) | *1.7.0* |  |
| :green_heart: | [Sparky V1](https://github.com/TauLabs/TauLabs/wiki/Sparky) | *1.6.0* |  |

| Status | [Midatronics](https://midatronics.com/) | Release | Comment |
| :---: | --- | :---: | :--- |
| :green_heart: | [SharkyMKR](https://midatronics.com/shop/development-boards/mkr-sharky-i/) | *1.7.0* |  |

## Next release

  See [milestones](https://github.com/stm32duino/Arduino_Core_STM32/milestones) to have an overview of the next release content.

## Troubleshooting

For question, support, ...,  you could submit a topic on the [stm32duino forum](http://stm32duino.com).

If you have any issue, you could [file an issue on Github](https://github.com/stm32duino/Arduino_Core_STM32/issues/new).

In any case, it always fine to search if your issue was not already existing before submit a new one.
