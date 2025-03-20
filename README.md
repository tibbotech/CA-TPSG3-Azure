# A sample project for cloud connectivity to Microsoft Azure IoT Hub with Tibbo Gen.3 TPP boards

This sample application is created to demonstrate the capability of TPP2G3 to connect securely to the cloud. The chosen server to connect is Microsoft Azure IoT Hub. 
This application simply samples the onboard temperature sensor (accessible via sys.boardtemp) every minute and sends it as a telemetry to Microsoft Azure IoT Central.

> [!TIP]
> Before using this test application, it is important to know that [AppBlocks](https://appblocks.io/), our no-code, in-browser, flowchart-based application development system for TPS supports connectivity to Azure and also Appblocks Cloud (ABC). AppBlocks automatically generates all the code required for this application. Therefore, we recommend using AppBlocks for your project. However, if you have an existing project and want to upgrade it to Gen.3 for secure cloud connectivity, using this test application might help you significantly.

## Pre-requisits
If you already have a Microsoft Azure account, you have worked before with IoT Central and you have an application, the path is easier. Just create your own device instance on IoT Central and bring its credentials, enter the web interface of the device and paste them, save and your device will connect to cloud and will be able to send telemetries to Azure.
In case you do not have an account, you can follow some of our documentation that has been created for OSS product line but you can use account procurement methods from there; here are some links:
* [Microsoft Azure Terminology and Configuration](https://docs.tibbo.com/oss_microsoft_azure_configuration)
* [Creating Microsoft Azure Account](https://docs.tibbo.com/oss_microsoft_azure_account)
* [Creating an Application](https://docs.tibbo.com/oss_iot_central_application)

## You Will Need

- A TPP2(G3) board.
- Optionally one Tibbit#10 for the power supply
- Optionally one Tibbit#18 to go along with Tibbit#10

## Connection 
Follow the diagram below for a minimal testing setup of the Tibbit#61:
![The Block diagram of TPP2(G3)](/Diagrams_and_Images/Connection_Diagram.png)


## The Test Program Flow
In *on_sys_init()*, 
1. Step 1
2. Step 2
3. Step 3

In *on_sys_timer()*, the following process is being repeated periodically:
The actions that are being done...

## Useful Links
* [Tibbo Website](https://tibbo.com)
* [Tibbo Project System (TPS)](https://tibbo.com/store/tps.html)
* [AppBlocks — Our No-code Platform](https://appblocks.io)
* [Microsoft Azure](https://azure.microsoft.com/en-us/)
* [Tibbo Support Center](https://tibbo.com/support.html)
