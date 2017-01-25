---
layout: master
include: default
---

### Overall Goals

The purpose of this session is to address a complex problem, split it into
sub-problems, divide the work, agree on interfaces, and to engage in
continued process of communication and revision towards solving the
problem.

The challenge is to precisely drive the robot to where we want. That
presumably means developing schemes for determining the robots current location, as
well as driving along a predictable path. This may sound straight
forward, but note that you don't have a GPS, only partial information about
the robots location. Our environment will consist of walls and boxes.

Some things we make try out include:

- Turn the robot to a given absolute angle.
- Drive in a straight line (Do you expect the robot to go straight by
  giving the same power to the two motors?).


### Hardware

You will be provided:

- [Makeblock Starter Robot Kit](http://www.makeblock.com/starter-robot).
- Various extra Makeblock beams, brackets, sensors, nuts, and screws.
- Raspberry Pi 3 with a pre-programmed SD card.
- Motor Shield for delivering regulated power to the Raspberry Pi.
- An extra sensor containing an accelerometer, a gyroscope, and a compass.
- RJ25 adaptor shield with header row for connecting I2C lines and cable for
  connecting the accelerometer, etc. to the Arduino.
- 7 Segment Display Shield to simplify protocol debugging, since the serial
  line will be occupied.
- Contacts, cables, and plastic parts to interface RPi with Makeblock.
- A shared access point.

You bring your own laptop to connect to the robot and to access available
documentation.


### Building the robot

We recommend to follow [our instructions](/teamwork/building/) but you are
welcome to experiment and create different robots.


### Arduino Software

To skip over the technicalities of designing the protocol between the
Raspberry Pi and the Arduino, you may start off with the our
[skeleton Arduino directory](https://github.com/neicnordic/ahm17.neic.nordforsk.org/tree/gh-pages/teamwork/arduino).
Most importantly this contains a driver for the extra shield containing
accelerometer, gyro, and compass.

You are of course free to change or replace any parts of the provided
software, and you should certainly extend it as needed.


### Raspberry Pi Network

We have set up a dedicated access point for connecting to the Raspberry Pis,
which also provides internet connectivity. The SSID is ahm2017 and with a
password to be provided.

The Pis are numbered from 1 to 4, and the corresponding IP numbers are:

- Robot 1: `192.168.1.11`
- Robot 2: `192.168.1.12`
- Robot 3: `192.168.1.13`
- Robot 4: `192.168.1.14`
