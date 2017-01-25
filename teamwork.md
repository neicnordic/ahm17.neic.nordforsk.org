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

#### Format

We want you to organize the work.  We assign to you some teams initially to
bootstrap the process.  You can then brainstorm what sub-problems needs to
be solved, and which ones can be worked on in parallel.  You can appoint a
leader and other roles as you feel necessary.  You can eventually contact
the other teams to regroup into workgroups addressing separate tasks.  These
workgrounps will then work together as needed to create the right
interfaces, so that you together will end up with a consistent solution.

Focus on relation between the problem and hand and the organization of the
work.  Redistribute people, regroup, merge, and split as you learn more
about the problem.

#### Detailed Goal Examples

Just to give an idea of what to aim for, consider the following challenges:

- Make a function to turn the robot to a given absolute angle.
- Make a function to drive in a straight line.  (Do you expect the robot to
  go straight be giving the same power to the two motors?)
- Drive the function in an equilateral triangle, attempting to get back to
  the starting point.
- Make a function which learns its position by measuring the distances to
  two walls, possibly driving up close enough first.
- Make a function which given an initial unknown location can drive to a
  provided location.
- Make a function which can locate a box.
- Make a function which can locate two boxes and park between them.

But note that before archiving most of the higher level goals, you will need
to learn to control the hardware and esp. get sensible results from the
sensors.  It's up to you to formulate intermediate challenges.  Don't expect
to solve all the higher level challenges, they are not as easy as they may
seem.

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
