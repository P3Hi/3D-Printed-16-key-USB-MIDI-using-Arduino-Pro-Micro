# 3D-Printed-16-key-USB-MIDI-using-Arduino-Pro-Micro

I was bored a bit so I made myself 3D Printed 16 key USB MIDI using Arduino Pro Micro.

I used Arduino Pro Micro, TTP229 16 Key Capacitive Keypad and one WS2812 LED. I designed casing using Adobe 123Design. All together was just around 5$.

Pro Micro is great because it can act as USB HID device and it support native MIDI over USB, so you don't need any cables/adapters for using it with your favorite software. For now, this device does nothing special, it just sends out MIDI data for 12keys.

- "noteOn(0, 47+key-4+octave, 110);"
- Two buttons I coded so they change octave.


This way you can use it as an instrument. At the end of the video, I mapped one button to stop playing all. But you can do whatever you want you just need an idea, I am thinking about extending it to be generic keyboard and send data to my IoT system running Node-Red. 

Sorry for crappy video, I don't have the right equipment and just two hands. I just wanted to show you how simple is to make cheap MIDI device :) 

# Code and setup the IDE
I did not write code for the touchpad. 

All is taken from this example: http://domoticx.com/arduino-keypad-4x4-aanraakgevoelig-ttp229/

For IDE I used Platform.IO and not Arduino Studio!
You need to install this two libraries into Platform.IO
- pio lib install "MIDIUSB"
- pio lib install "Adafruit NeoPixel"

Project should be easy to compile using Arduino Studio just install the same two libraries.

Check this site to learn more about the touchpad and how to setup multitouch if you need it.
https://www.robotics.org.za/TTP229-MOD

See more on Hackster.IO!
https://www.hackster.io/p3hi/3d-printed-16-key-usb-midi-using-arduino-pro-micro-c6c23e

# Check demonstration here
[![Demonstration](https://img.youtube.com/vi/_5QUpAhMLr8/0.jpg)](https://www.youtube.com/watch?v=_5QUpAhMLr8)
