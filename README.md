# Arduino_Bluetooth
This ties into the youtube video explaining how to connect a Bluetooth unit to an Arduino.

In this particular video I use a cheap HC-06 but there are many similar units. I ran out before this video, but the HC-10 is a better unit with BLE 4.0 which allows communications with iPhones and recent Androids. This particular unit will only communicate with desktops, laptops, and other similar devices.

In this particular example I use the SoftwareSerial library. This then moves the RX, TX off the RX, TX pins on the Arduino. The benefit of this is that the bluetooth can interfere with programming the Arduino via the USB as the TX, RX pins are the same as what is used while uploading a sketch. By moving to different pins this problem goes away. 

Not all pins can be used for SoftwareSerial and it does impose a slight overhead. If memory is tight it is not necessary. 

The accompanying YouTube video is:

https://www.youtube.com/watch?v=3tcn496oxnk

Feel free to contact me with any questions or suggestions.
