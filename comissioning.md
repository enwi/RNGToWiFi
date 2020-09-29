# First comissioning of `RNG to WiFi`

## Step 1
Connect `RNG to WiFi` with an `RJ12` cable to your Charge Controllers `RS232` port. 
The LED on `RNG to WiFi` will light up solid. 
Once the LED starts blinking at a 2 second interval you can continue with the next step.

## Step 2
Connect your phone/tablet/pc to the WiFi network called `rngbridge`. 
You can also scan this QR code to connect to the WiFi network.

![WiFi QR](https://github.com/enwi/RNGToWiFi/blob/master/images/qr_wifi_rngbridge.png)

## Step 3
Once connected open up a browser, type in the URL `192.168.1.1` and open the website (hit enter).
After the page loaded, you are presented with the user interface of `RNG to WiFi`.
Alternatively you can scan this QR code to open the browser with the correct URL.

![WiFi IP QR](https://github.com/enwi/RNGToWiFi/blob/master/images/qr_url_192.168.1.1.png)

If you want to use `RNG to WiFi` as standalone aka in access point mode you are done with comissioning now. 
If you want to connect `RNG to WiFi` with your local WiFi network continue with step 4.

## Step 4
Click on the `WiFi` tab to open the WiFi settings.
In the field `SSID` enter the name of the WiFi network you want `RNG to WiFi` to connect with.
In the field `Password` enter the password of the WiFi network.

> Note that the SSID and Password are limited to 32 characters

Verify that the `SSID` and `Password` are correct and enable the `Enable` switch to enable the client mode.
After that `RNG to WiFi` will scan all nearby WiFi networks and if a network with the correct SSID is found, connect to it. 

> If no matching WiFi network is found or the password is wrong `RNG to WiFi` will stay in the access point mode and will try to reconnect every 5 seconds

## Step 5
Once `RNG to WiFi` has connected successfully with your local WiFi network you can access the user interface from your browser like in `Step 3`.
To make things easier you can use the URL `http://rngbridge.local` or again scan the QR code below.
![WiFi URL QR](https://github.com/enwi/RNGToWiFi/blob/master/images/qr_url_rngbridge.png)

> On some phones or browsers you might run into the issue that the page won't load with the error `DNS_PROBE_FINISHED_NXDOMAIN`.
> In this case I recommend using a different browser or device.

If everything worked out fine you are now setup. For infos on how to setup `MQTT` or `PVOutput` please take a look at the respective guides [MQTT](https://github.com/enwi/RNGToWiFi/blob/master/mqtt.md) and [PVOutput](https://github.com/enwi/RNGToWiFi/blob/master/pvoutput.md).