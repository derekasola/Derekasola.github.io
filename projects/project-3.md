---
layout: project
type: project
image: images/googlemaps (2).jpg
title: Location Alarm
permalink: projects/Location Alarm
# All dates must be YYYY-MM-DD format!
date: 2019-07-01
labels:
  - Android
  - Java
  - Google Maps API
summary: An alarm app to wake me up when I take long bus rides.
---

<img class="ui medium right floated rounded image" src="../images/prox1.jpg">
 I use google maps API to get user location and have the user select location of interest with a bubble that changes in size. Once the user comes within the user specified bubble, an alarm will trigger. Current version doesn't use location data from the API to search for places of interest.

 Permission request for location services:
 ---

 ```Java
 while (ActivityCompat.checkSelfPermission(this, Manifest.permission.ACCESS_FINE_LOCATION)
                != PackageManager.PERMISSION_GRANTED
                && ActivityCompat.checkSelfPermission(this, Manifest.permission.ACCESS_COARSE_LOCATION)
                != PackageManager.PERMISSION_GRANTED) {

            ActivityCompat.requestPermissions(this, new String[]{Manifest.permission.ACCESS_FINE_LOCATION}, 1);

        }
 ```

[Google Maps Docs](https://developers.google.com/maps/documentation/javascript/tutorial), [Git Repository](https://github.com/derekasola/ProxAlarm2)
