# Azure IoT Central Concepts and Features

- [Personas](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central#personas): There are four defined personas who interact with an IoT Central application:
  - Solution builder: responsible for defining the types of devices that connect to the application and customizing the application for the operator.
  - Operator: manages the devices connected to the application.
  - Administrator: responsible for administrative tasks such as managing user roles and permissions within the application.
  - Device developer: creates the code that runs on a device or IoT Edge module connected to your application.

- Types of device:
  - [Standalone device](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central-developer#standalone-device): Anything that has a sensor attached to it and can transmit data to IoT Central.
  - [Gateway device](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central-developer#gateway-device): manages one or more downstream devices that connect to your IoT Central application. You use IoT Central to configure the relationships between the downstream devices and the gateway device.
  - [Edge device](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central-developer#edge-device): connects directly to IoT Central, but acts as an intermediary for other devices known as leaf devices. An edge device is typically located close to the leaf devices for which it's acting as an intermediary.

- [Azure IoT Edge](https://docs.microsoft.com/en-us/azure/iot-edge/about-iot-edge): physical device that moves cloud analytics and custom business logic to the edge; consists of IoT Edge modules, IoT edge runtime, and cloud-based interface

- [Azure IoT Hub](https://docs.microsoft.com/en-us/azure/iot-hub/about-iot-hub): foundation of Azure IoT Central and acts as a cloud gateway that enables device connectivity.

- [Rules](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-configure-rules): a customizable tool that trigger on actively monitored events from connected devices.

- [Actions](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-use-action-groups): In Azure IoT Central, you create rules to run actions when a condition is met.

- [Jobs](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-run-a-job):
enable operators to do bulk updates to device properties and run commands

- [Dashboards](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-set-up-template#generate-default-views): provide a customizable UI to monitor device health and telemetry

- [Device template](https://docs.microsoft.com/en-us/azure/iot-central/core/concepts-architecture#metadata-management): define the capability and properties of types of device
  - [Device capability models](https://docs.microsoft.com/en-us/azure/iot-pnp/overview-iot-plug-and-play):  specify the capabilities of a device such as the telemetry it sends, the properties that define the device state, and the commands the device responds to.
  - Cloud properties: specify the properties IoT Central stores for a device. These properties are only stored in IoT Central and are never sent to a device.
  - Views: specify the dashboards and forms the builder creates to let the operator monitor and manage the devices.

- [Data export](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-export-data): enable builders to export IoT Central data continuously to Azure Event Hubs, Azure Service Bus, or Azure Blob storage instances

- [RBAC](https://docs.microsoft.com/en-us/azure/iot-central/core/howto-manage-users-roles): An administrator can define access rules for an Azure IoT Central application using one of the predefined roles or by creating a custom role.

- [Azure IoT Hub Device Provisioning Service (DPS)](https://docs.microsoft.com/en-us/azure/iot-dps/about-iot-dps): IoT Central uses DPS to manage the connection process. A device first connects to DPS to retrieve the information it needs to connect to your application.

- [Security](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central-developer#security): the connection between a device and your IoT Central application is secured using either [shared access signatures](https://docs.microsoft.com/en-us/azure/iot-central/core/concepts-get-connected#connect-devices-at-scale-using-sas) or industry-standard [X.509 certificates](https://docs.microsoft.com/en-us/azure/iot-central/core/concepts-get-connected#connect-devices-using-x509-certificates).

- [Communication protocols](https://docs.microsoft.com/en-us/azure/iot-central/core/overview-iot-central-developer#communication-protocols): Communication protocols that a device can use to connect to IoT Central include MQTT, AMQP, and HTTPS. Internally, IoT Central uses an IoT hub to enable device connectivity.