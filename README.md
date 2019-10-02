
Webapp clone of the Azure real time sensor data visualization
-------------------------------------------------------------


Simple clone app of the official [web-app](https://github.com/Azure-Samples/web-apps-node-iot-hub-data-visualization.git) from the official docs [iot-hub-live-data-visualization-in-web-app](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-live-data-visualization-in-web-apps).

The set-up and modification for the Azure account is given in the official tutorial. 

This repository is just a reference, that highlihgt relevant details neccessary for a working example app. These points are contained in the comments in the relevant configuration files.  

The sensor data is sent to azure from `send_sensor_data_to_azure/dht_temp.js`, which requires the installations of:

 ```bash
sudo npm install --unsafe-perm node-dht-sensor
npm install azure-iot-device
npm install azure-iot-device-mqtt
```

Note

Modify the line in the file `web-apps-node-iot-hub-data-visualization/scripts/event-hub-reader.js` by adding the IoThowner connection string located in IoTHub "Share access policies" iothubowner connectionstring, which is not the device connection string.
