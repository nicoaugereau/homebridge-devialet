# delta-homebridge



Install Homebridge
```
sudo npm install -g https://github.com/NorthernMan54/homebridge
```


Homebridge + Alexa

Add ssdp property to the bridge section of the config.json and ensure the value is set to 1900 to complete the installation.
```
 "bridge": {
    "name": "Example",
    "username": "CC:22:3D:E3:CE:31",
    "port": 51826,
    "pin": "031-45-154",
    "ssdp": 1900
},
```
Run Homebridge as you did before with the homebridge command and it will now expose your devices to an Echo on the same network.

Now that devices are discoverable, Alexa can be asked to find them. This can either be done via the app under the Smart Home > Devices section or by saying "Alexa, discover devices"
