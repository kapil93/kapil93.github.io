---
layout: project_with_company
title:  "Navigation"
date:   2016-11-12 11:54:46
categories:
- project
img: navigation.jpg
thumb: thumb02.jpg
carousel:
- navigation.jpeg
company: Witworks Consumer Technologies
---
## Navigation
--------------

### Overview
A navigation app for [Blink Smartwatch](https://blink.watch) which provides turn by turn directions.

Travel modes it supports include driving, walking and transit. Voice commands are used for destination input.

<br>

### Challenges I faced
The primary blocker in the course of making this project was the absence of GPS tracker and Google Play Services in the watch.

Google Directions API was used for getting the directions to destination and utility classes from various libraries were used for calculating distance to next leg, estimated time of arrival, the logic for rerouting and the detection of arrival at destination.

Also one of our prime concerns remains the battery efficiency as the watch has even limited resources than a smartphone.

As the watch does not have Wi-Fi, it gets internet from the phone via Bluetooth Classic which takes a toll on the battery. So hitting the directions API was kept to a minimum, just one time in best case scenario.

GPS data from the phone was sent to the watch via BLE which consumes much less battery but has a relatively low bandwidth as compared to Bluetooth Classic.