# A sample project for cloud connectivity to Microsoft Azure IoT Hub with Tibbo Gen.3 TPP boards

This sample application is created to demonstrate the capability of TPP2(G3) to connect securely to the cloud. The chosen server to connect is Microsoft Azure IoT Hub. 
This application simply samples the onboard temperature sensor and accelerometer values every minute and sends it as a telemetry to Microsoft Azure IoT Central.
The sample also has a web server that allows you to simply input the credentials of Azure IoT Central.

> [!TIP]
> Before using this test application, it is important to know that [AppBlocks](https://appblocks.io/), our no-code, in-browser, flowchart-based application development system for TPS supports connectivity to Azure and also Appblocks Cloud (ABC). AppBlocks automatically generates all the code required for this application. Therefore, we recommend using AppBlocks for your project. However, if you have an existing project and want to upgrade it to Gen.3 for secure cloud connectivity, using this test application might help you significantly. Also, note that the base code for this application is generated by AppBlocks!

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

## The Configuration and Testing
1. Build and load the application to the TPP2(G3) board.
2. Find out the IP of the device; note that this application runs DHCP and will get an IP from your router's DHCP server.
3. Open a browser tab and type the IP address and open the page.
4. Go to your Microsoft IoT Central Application and create a device instance and attach a template to it. You can download our proposed template [here](/Resources/TPS_G3_V0.json) and import it to your Azure IoT Central Application.
5. Press connect and you can see the credentials of the cloud instance.
6. Enter the device credentials you have received from IoT Central in the corresponding fields and press the save button.
7. Go to your IoT Central Device instance and check for telemetries in "Raw data" pane. You should be able to see telemetries (json format) that includes your sensor values. If you like to visualize your data, you can refer to this [tutorial](https://docs.tibbo.com/oss_visualizing_data); however, it is important to be mentioned that this instructions are not built for this device and are for OSS.

Feel free to contact _support@tibbo.com_ in case you have questions.

## Useful Links
* [Tibbo Website](https://tibbo.com)
* [Tibbo Project System (TPS)](https://tibbo.com/store/tps.html)
* [AppBlocks — Our No-code Platform](https://appblocks.io)
* [Microsoft Azure](https://azure.microsoft.com/en-us/)
* [Tibbo Support Center](https://tibbo.com/support.html)
