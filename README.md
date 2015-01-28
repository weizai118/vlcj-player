vlcj-player
===========

The vlcj-player is a media player application built using vlcj with a Swing
rich-client user interface. 

The main goal of the project is to provide an extensive demo application 
showing how to build media players with vlcj, and to include as many features
of vlcj as possible.

Generally the vlcj-player tries to match the Qt interface of VLC with as many
of the same features implemented as possible.

However, it is not possible to get a 100% like-for-like implementation since
LibVLC, used by vlcj, exposes only a sub-set of the total functionality of VLC. 

Screenshot
----------

![vlcj-player](https://github.com/caprica/vlcj-player/raw/master/doc/vlcj-player.png "vlcj-player")

Features
--------

 - audio player
 - video player
 - full-screen
 - audio equalizer
 - video adjustments
 - title selection
 - chapter navigation
 - audio track selection
 - video track selection
 - subtitle track selection
 - load external subtitle file
 - change audio device
 - change playback speed
 - capture and display native logs
 - capture and display video surface debug messages (e.g. to test mouse and keyboard events still work)
 - volume controls
 - mute
 - zoom/scale
 - aspect ratio
 - crop
 - always on top
 - video snapshots
 - redirect native output streams (on Linux)

...and a whole bunch of other nifty stuff.
 

Status
------

This project is currently a work-in-progress.

The core of the application is there and is usable, but there are significant
features missing and a whole bunch of FIXME and questionable code.

It is however a good example for how to build media players with vlcj, and has
more time and care invested in it than most of the individual vlcj test 
examples.

If you execute "mvn install" or "mvn package", you will get a distribution
package that you can unpack. This will give you the vlcj-player application jar
and all of the dependencies - you can simply execute `java -jar vlcj-player-1.0.0-SNAPSHOT.jar`
and the application should start.

On the other hand, just run it from an Eclipse project.

vlcj Dependency
---------------

This project currently requires a bleeding edge vlcj-3.2.0-SNAPSHOT, so you
will have to build vlcj yourself from the maven project until vlcj-3.2.0 final
release is made to Maven Central.

License
-------

The vlcj-player project is provided under the GPL, version 3 or later.
