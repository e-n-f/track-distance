track-distance
==============

Calculate how far and how fast people travel in each GPX track.

    $ curl -LO http://planet.osm.org/gps/gpx-planet-2013-04-09.tar.xz
    $ xzcat gpx-planet-2013-04-09.tar.xz | tar xvf - gpx-planet-2013-04-09/identifiable
    $ cd gpx-planet-2013-04-09
    $ find identifiable -type f -print | sort | xargs ./get-track-distance > track-distance
    $ sort -n track-distance | ./spread-distribution > trips-per-distance
    $ gnuplot plot-3power > 3power.ps
