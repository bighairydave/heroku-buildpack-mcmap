Heroku buildpack: MineCraft Map
=======================

This buildpack will provide MineCraft world in Google Map format using [overviewer](http://overviewer.org/).

Usage
-----

Example usage:

    $ ls
    data level.dat players region

    $ heroku create --stack cedar --buildpack http://github.com/samitheberber/heroku-buildpack-mcmap.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> MineCraft Map app detected
    -----> Found a level.dat

The buildpack will detect that your app has a `level.dat` in the root. World data is transformed to Google Map using Overviewer.
