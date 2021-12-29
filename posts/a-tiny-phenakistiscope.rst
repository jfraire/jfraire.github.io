.. title: A tiny phenakistiscope
.. slug: a-tiny-phenakistiscope
.. date: 2021-12-28 00:15:01 UTC+01:00
.. tags: phenakistiscope
.. category: electronics
.. link: 
.. description: A phenakistiscope circuit!
.. type: text

The phenakistiscope is a rotating disk that produces short animations. It was invented in the 19th century, and the disks from that time are really beautiful. The animations they create are intriguing. In this `series </posts/phenakistiscope>`_ we look at a few of the ideas that result in these captivating works of art.

A different kind of charm
-------------------------
I know. The XIX century animations are charming. Seeing the rotating disks through their slits, in front of a mirror, would transport you to another world, another ambiance of high hats, beautiful dresses, spectacles… a refined atmosphere. And I am about to break all this by talking about servo-motors, LEDs and micro-controllers.

But bear with me. We are talking about a little ATtiny85 micro-controller. Only 8 terminals in a sweet thru-hole package. This tiny fellow can use a continuous-rotation servo-motor, some potentiometers, and a bunch of LEDs to replace the slits and the mirror. And the best part, it will let you see the animations at the same time as your kids.

The idea is simple: The servo-motor spins the disk while the LEDs blink. The disk will advance a certain angle between two LED flashes. If this angle coincides with the design of the disk, the animation will come to life!

And this is where the two potentiometers come in: One of them will let you change the speed of the servo-motor. The other potentiometer will change the time between the flashes of the LEDs.

.. image:: /images/phenakistiscope.jpg
    :height: 284px
    :width: 350px
    :alt: The phenakistiscope assembled in a tea can

A brief description of the program and the circuit
--------------------------------------------------

The ATtiny85 is a nice piece of micro-controller. The program configures a timer to produce the PWM signal  for the servo-motor, another timer for the LEDs, and the ADC to read the two potentiometers. Then, it uses the readings of the potentiometers to change the limits of the timers. And that’s it! 

You can see the listing of the program below. It has more comments than code because the actual code is… cryptic. You should check the `datasheet <https://www.microchip.com/en-us/product/ATtiny85>`_ to make sense of it. It is almost pure configuration. The only logic is there to copy the potentiometer readings to the timers.

.. listing::  phenakistiscope_attiny.c c

In terms of the circuit, the micro-controller doesn’t require much. The circuit has just a voltage regulator, and terminals for the potentiometers, servo-motor, and LEDs. Only one pin is used for the LEDs. I should have put a transistor instead.

I put everything in a repository, in GitHub. Even the Gerber files.

.. image:: /images/open_phenakistiscope.jpg
    :height: 444px
    :width: 250px
    :alt: The phenakistiscope circuit assembled in a tea can

My own animated disk!
---------------------

And this is my first animated disk. The pleasure to see it animated is unbelievable. It lacks the charm of the XIX century but has a reminiscence of aliens and cows.

.. image:: /images/cow_abduction.gif
    :height: 395px
    :width: 400px
    :alt: An animated disk of aliens abducting cows

And here it is, the real thing:

.. youtube:: Ikgw9VhqUUA



About this series
-----------------

This is the fifth and last article about the phenakistiscope. In this short series, I describe some of the ideas used to animate the disks. The first article is `here </posts/phenakistiscope>`_.

