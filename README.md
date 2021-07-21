# Start Here

Once you have your login details, go to [Aeroire Web Dashboard](https://aeroire.itspot.org/).

Login with your credentials. You will be taken to the hosts page. This is where you will see all hosts associated with your account. Think of hosts like a controller to control electrical devices. For example a raspberry Pi can be a host with multiple devices (like, relays, button, lights) attached to it.

Currently your list is empty so, the first step is to create a new HOST.

1) Click on `Add new Host` Button
2) Give your host a name
3) After you click on `ADD` you will be shown a host key, note this down. **KEEP THIS SECRET!**

You will now see a new host added to your list. The status is `UNKNOWN` and the details button is disabled. This is an indicaiton that you need to setup the host.

Setup the host using the guide for the [Raspberry Pi](https://github.com/aroire/raspberrypi-host/wiki/Getting-Started). Once your host is setup and you can see the online status in the dashboard, its time to add devices to your host.

## Add Devices
Now will be a good time to attach an LED or some output device to a free gpio pin. As such:

![raspberry pi with LED](https://cdn.shopify.com/s/files/1/0176/3274/files/LEDs-BB400-1LED_bb_grande.png?6398700510979146820)

Open the details view of your host. Then click on `Devices` >> `Add Device`.

1) Give your device a name. This will also be the name which will be used in Alexa and other voice assistants
2) Select device type of 'LIGHT'
3) Select a pin for your device. Use the diagram below to select a **free** pin!


![alt text](https://www.bigmessowires.com/wp-content/uploads/2018/05/Raspberry-GPIO.jpg)

## NOTE
Remember to use the pysical pin numbers and not gpio numbers. EG use pin#`3` instead of **GPIO**`2`

## Test your setup
You will now see that your device is visible in the devices table. Click `VIEW` button to go to device details. If you are able to see details about your device, you have successfully added a new device. The next step is to stop the host program and start it again using the commands provided [HERE](https://github.com/aroire/raspberrypi-host/wiki/Getting-Started). Once your host is online again go to your device page and try to power on and off your device using the `ON` and `OFF` buttons in the device page.
