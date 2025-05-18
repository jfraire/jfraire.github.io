.. title: Animating radial movements
.. slug: animating-radial-movements
.. date: 2021-12-15 22:55:14 UTC+01:00
.. tags: phenakistiscope
.. category: electronics
.. link: 
.. description: Radial movements in the phenakistiscope
.. type: text

In the `first article of this series </categories/phenakistiscope>`_ we discussed about the phenakistiscope, a rotating disk that produces short animations. In that post we saw a running horse and how it was made to move forward by having less frames than disk stops. Movement was *tangential*. In this article, we will talk about *radial* movements.

.. TEASER_END

Animating radial movements
--------------------------

To make a feature move in a radial, straight line, start by placing the first frame in the disk. For example, put your image close to the border of the disk. Then, turn the disk by the angle of the animation (30° for 12 frames, for example) and draw your image in the next frame, *along the line you want it to follow*. Continue until you have all the frames you want. At the end of this exercise, your images will describe a spiral!

For some thought food, see what is an `archimedean spiral <https://en.wikipedia.org/wiki/Archimedean_spiral>`_. 

This disk from 1833 shows a man feeding a frog with some red balls. The balls are drawn along a spiral, but in the animation, you will see them falling along a radial straight line.

.. image:: /images/frogs_feeding.png
    :height: 300px
    :width: 300px
    :alt: Disk from 1833 that is animated when spun

.. image:: /images/frogs_feeding.gif
    :height: 300px
    :width: 300px
    :alt: Animated disk of red balls moving along straight lines

So far, we have discussed two movements: Tangential and radial. `In the next article </posts/a-balancing-monkey-and-a-jumping-zebra>`_ we will talk about objects that move “up and down”, radially. 

About this series
-----------------

This is the second article about the phenakistiscope. In this short series, I describe some of the ideas used to animate the disks. The first article is `here </posts/phenakistiscope>`_.

The image used above can be found in `the library of congress of the United States <http://loc.gov/pictures/resource/cph.3g08091/>`_ and it is in the public domain.
