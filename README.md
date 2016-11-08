# dutch-ferries

This repository contains an open GTFS-feed of the smaller Ferries in the Netherlands. It is still a work-in-progress. The frequencies related to the trips are auto-generated and the stops and the shapes still require manual checking.

## Edit the GTFS

GTFS files describe trips in a set of simple csv files according to the specification that can be found here: https://developers.google.com/transit/gtfs/reference/

They can be manually adjusted (be sure to choose unique id's for the different entities) or can be edited with specific GTFS editors (find the best on Google).

## Try the GTFS

If you would like to try out the current state, download the zip of the master branch: https://github.com/plannerstack/map-data-issues/archive/master.zip and run it in your favorite GTFS application.

Ok, it's not that easy, as GitHub decides to add an extra directory in the zip file and GTFS expects no sub-directories to be in there, so after downloading, you still need to re-zip the files again without the sub-directory:

```
wget "https://github.com/plannerstack/map-data-issues/archive/master.zip" -O dutch-ferries-master.zip
unzip dutch-ferries-master.zip
cd dutch-ferries-master/
zip gtfs.zip .
```

Less elegant, but works.
