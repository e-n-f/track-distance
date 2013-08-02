track-distance
==============

Calculate how far and how fast people travel in each GPX track.

    $ xzcat gpx-planet-2013-04-09.tar.xz | tar xvf - gpx-planet-2013-04-09/identifiable
    $ find identifiable -type f -print | sort | xargs ./get-track-distance > track-distance
