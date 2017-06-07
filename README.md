> Trying to get started on TI microPs. I have a feeling this is the wrong place to start but...it's a start. Will be sure after a few hours of eyeballing. 

# Introduction

These examples and demos are for **TI SimpleLink CC2640R2 SDK 1.35.00.33**

This repository contains **experimental** *Bluetooth&reg;* 5 and
*Bluetooth&reg;* 4.2 Low Energy sample applications for Texas Instruments'
SimpleLink CC2640R2 SDK. These examples have not been validated as
production-ready.

**Do not** use GitHub's bug tracking feature for support. For inquiries, see the
[Bluetooth&reg; low energy Forum](https://e2e.ti.com/support/wireless_connectivity/bluetooth_low_energy/f/538).

To use the examples and tools in this repository, please download and install
the [SimpleLink CC2640R2 SDK](http://www.ti.com/ble-stack) **first**, and if
necessary [buy an evaluation kit](http://www.ti.com/tool/launchxl-cc2640r2).

For other hardware and software resources,
[please visit our wiki](http://www.ti.com/ble-wiki). If you have any questions
please refer to the [FAQ page](docs/faq.md).

## Change Log

### 1.35.02.02
* BLE5-Stack: Added Serial Port Profile (SPP) Server/Client
* BLE-Stack:  Added Serial Port Profile (SPP) Server/Client

### 1.35.01.01
* BLE5-Stack: Added Long Range Demo (Central/Peripheral)
* BLE5-Stack: Added CCS projects for Throughput Demo
* BLE5-Stack: Throughput Demo improvements

### 1.35.00.00
Initial offering of Simplelink CC2640R2 SDK examples.
* BLE5-Stack: Throughput Demo (Central/Peripheral)

## Installation

This repository can be cloned and tracked using Git. For instructions on how to
clone a repository from Github please refer to this guide:
[Clone from Github](https://help.github.com/articles/cloning-a-repository/)

For users who are unfamiliar with Git, there is the option of downloading the
contents of the repository as a zip file. See instructions below.

1. Click the green "Clone or download" button
1. Select "Download ZIP" option
1. Zip folder will appear in your Downloads folder

This repository can be cloned/download anywhere on your computer. There is a
dependency between this repository and the SimpleLink CC2640R2 SDK install
location.

By default the SimpleLink CC2640R2 SDK will install to:

    C:\ti\simplelink_cc2640r2_sdk_1_35_00_33

If the Simplelink CC2640R2 SDK must be installed to a different location, then
see the [FAQ page](docs/faq.md) for IDE specific instructions for changing
environment variables.

## Required Tools

Similar to the Simplelink CC2640R2 SDK, the examples in this repository support
the CCS and IAR toolchains. Please pay careful attention to versions of these
tools, the supported version are listed below. Using a non supported version is
untested and may result in unexpected behavior.

* CCS v7.1.0 with TI ARM Compiler v16.09
* IAR for ARM v7.80.3

For more information on toolchain setup, please refer to our
[FAQ page](docs/faq.md).

## FAQ

The [FAQ page](docs/faq.md) will try to address some of the common questions
related to the ble_examples repo.

## Examples / Demo List

### Bluetooth 5 Throughput Demo

This is a 2 part demo where a throughput\_central and throughput\_peripheral
connect with one another, demonstrating the BLE5-Stack's 1 Mbps, 2 Mbps, 1+2
Mbps, and Coded PHYs.

* throughput\_central
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_central/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_central/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_central/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_central/src)
* throughput\_peripheral
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_peripheral/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_peripheral/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_peripheral/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/throughput_peripheral/src)

### Bluetooth 5 Long Range Demo

This is a 2 part demo where a longrange\_central and longrange\_peripheral
connect with one another, demonstrating the BLE5-Stack's long range capabilities
using the Coded PHY (S8).

* longrange\_central
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_central/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_central/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_central/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_central/src)
* longrange\_peripheral
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_peripheral/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_peripheral/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_peripheral/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/longrange_peripheral/src)

### Serial Port Profile (SPP) BLE Examples

This is a 2 part example where a spp\_ble\_client and spp\_ble\_server connect
with one another and exchange data over UART.

The demo supports Bluetooth 5 demonstrating the BLE5-Stack's new high speed 2Mbps PHYs:

* spp\_ble\_client
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_client/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_client/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_client/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_client/src)
* spp\_ble\_server
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_server/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_server/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_server/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/ble5apps/spp_ble_server/src)

The example also supports Bluetooth 4.2 demonstrating the BLE-Stack's Data Length
Extension with OAD support:

* spp\_ble\_client
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_client/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_client/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_client/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_client/src)
* spp\_ble\_server
    * [Documentation](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_server/readme.md)
    * [IAR Project Files](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_server/tirtos/iar)
    * [CCS Project Files](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_server/tirtos/ccs)
    * [Source](examples/rtos/CC2640R2_LAUNCHXL/bleapps/spp_ble_server/src)

## References

The following reference pages may be helpful during general Bluetooth Low
Energy development. New users of the Simplelink CC2640R2 platform and Bluetooth
5 development are encouraged to read the
[BLE5-Stack User's Guide][BLE5-Stack].
Users developing Bluetooth 4.2 applications are encouraged to read the
[BLE Software Developer's Guide][BLE-Stack].

As an additional resource, users are encouraged to complete the
[SimpleLink Academy](http://software-dl.ti.com/lprf/simplelink_academy/overview.html)
training.

Other resources can be found below:

* [BLE wiki](http://www.ti.com/ble-wiki)
* [BLE E2E Page](www.ti.com/ble-forum)

[BLE5-Stack]: (http://software-dl.ti.com/lprf/ble5stack-docs-latest/docs/ble5stack/ble_user_guide/html/cc2640/index.html)
[BLE-Stack]:  (http://software-dl.ti.com/lprf/sdg-latest/html)
