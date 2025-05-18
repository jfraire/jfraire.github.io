.. title: Playing with spirals
.. slug: playing-with-spirals
.. date: 2021-12-22 22:48:15 UTC+01:00
.. tags: phenakistiscope
.. category: electronics
.. link: 
.. description: Sprials in the phenakistiscope
.. type: text
.. has_math: true

In this `series of posts </categories/phenakistiscope>`_ we look at a few of the ideas behind an early animation toy, the phenakistiscope. And now it is time to explore
spirals that perform more than one turn per disk rotation. These spirals will add a new dimension to our animations.

.. TEASER_END

Spirals and more spirals!
-------------------------

In the `first article </posts/phenakistiscope>`_ of the series, we saw how a spiral forms a radial movement when animated in a phenakistiscope. Actually, the polar equation of a spiral that starts in the center of the disk looks very similar to that of a line in Cartesian coordinates: :math:`r = m \theta`. It simply says that the radius changes in proportion to the rotation angle.

So, if we put stuff in such a spiral, it will move along radial lines. Now, if the radius increments slowly for each change in angle, the spiral can last for several complete turns before it reaches the brim of the disk. In the disk below, the spiral completes at least 7 turns of 20 frames each. The visual effect is stunning:

.. image:: /images/circles-spiral.png
    :height: 300px
    :width: 300px
    :alt: Disk with colorful circles ordered along a spiral

.. image:: /images/circles-spiral.gif
    :height: 300px
    :width: 300px
    :alt: Animated disk with colorful circles ordered along a spiral

The same idea is at work in the next, beautiful disk:

.. image:: /images/phena_greendemons_small.gif
    :height: 300px
    :width: 300px
    :alt: Animated disk of monsters

An homage to Joseph Plateau, the inventor of the phenakistiscope
----------------------------------------------------------------

Google produced a set of *doodles* to celebrate Joseph Plateau and his early animations. I find the disk below very interesting. It combines two movements: The frying pan is moving up and down because its frames are drawn along a circle. But the pancake in the animation seems to move in a parabolic trajectory as dictated by the laws of physics. Note how it does not move in a circle, nor in a spiral! Also, the pancake is not moving from the center, but from the brim of the disk.

.. image:: /images/plateau-google.png
    :height: 225px
    :width: 223px
    :alt: Disk drawn by Google in homage of Joseph Plateau

.. image:: /images/plateau-google.gif
    :height: 225px
    :width: 223px
    :alt: Disk drawn by Google in homage of Joseph Plateau, animated

About this series
-----------------

This is the fourth article about the phenakistiscope. In this short series, I describe some of the ideas used to animate the disks. The first article is `here </posts/phenakistiscope>`_.

The `next article </posts/a-tiny-phenakistiscope>`_ will discuss a little machine to animate cardboard disks!
