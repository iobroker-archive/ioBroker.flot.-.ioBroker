![Logo](admin/flot.png)
ioBroker.flot
=================

[![NPM version](http://img.shields.io/npm/v/iobroker.flot.svg)](https://www.npmjs.com/package/iobroker.flot)
[![Downloads](https://img.shields.io/npm/dm/iobroker.flot.svg)](https://www.npmjs.com/package/iobroker.flot)

[![NPM](https://nodei.co/npm/iobroker.flot.png?downloads=true)](https://nodei.co/npm/iobroker.flot/)

Draw charts with [flot](http://www.flotcharts.org/)

![Example](img/example.png)

To use the charts one of the history adapters is required: history, sql or InfluxDB

To **edit** created chart again, you should replace index.html with edit.html and call this link in browser, e.g:

http://localhost:8082/flot/**index**.html?l%5B0%5D%5Bid%5D=system.adapter.admin.0.memRss

to

http://localhost:8082/flot/**edit**.html?l%5B0%5D%5Bid%5D=system.adapter.admin.0.memRss

## Changelog
### 1.3.2 (2016-06-13)
* (bluefox) add settings for border color and border width
* (bluefox) make splines work 

### 1.3.1 (2016-06-07)
* (bluefox) add spline file

### 1.3.0 (2016-05-29)
* (bluefox) add animation
* (bluefox) remove smoothing, because does not work
* (bluefox) try to add splines, but it does not work always

### 1.2.5 (2016-05-28)
* (bluefox) do not include nulls by smoothing

### 1.2.4 (2016-05-27)
* (bluefox) show edit button

### 1.2.3 (2016-05-25)
* (bluefox) fix digits after comma
* (bluefox) fix start and finish points

### 1.2.2 (2016-05-22)
* (bluefox) change default aggregation name
* (bluefox) add units in tooltip

### 1.2.1 (2016-05-13)
* (bluefox) implement loading indicator

### 1.2.0 (2016-05-05)
* (bluefox) implement zoom and pan
* (bluefox) support ms
* (bluefox) support m4
* (bluefox) support of pan and zoom on touchable devices
* (bluefox) support of 3 types of "null" handling: use nulls, use last value instead of null, use 0 instead of 0
* (bluefox) update interval in seconds
* (bluefox) smoothing and "after comma" per variable

### 1.1.0 (2016-04-09)
* (bluefox) change splash screen
* (bluefox) ignoreNull per variable
* (bluefox) fix x axis

### 1.0.0 (2016-04-09) 
* (bluefox) enable editing of created charts
* (bluefox) enable set of label colors
* (bluefox) enable set of window background

### 0.2.6 (2016-02-24)
* (Pmant) remove ignore null per state

### 0.2.5 (2016-02-14)
* (Pmant) add ignore null per state
* (Pmant) change commonYAxis per state

### 0.2.4 (2016-01-31)
* (ldsign) Title/help attribute for lineWidth and ShadowSize table head
* (ldsign) option for shadowSize
* (nobodyMO) Add option commonYAxis
* (bluefox) add favicon and title

### 0.2.3 (2016-01-26)
* (ldsign) user selectable time (hours/minutes) for static timeArt

### 0.2.2 (2015-12-17)
* (bluefox) fix SelectID for safary

### 0.2.1 (2015-12-14)
* (Smiling_Jack) support of new History concept
* (Smiling_Jack) new editor & working on axis
* (bluefox) add onchange aggregation
* (Smiling_Jack) add ignoreNull
* (Smiling_Jack) working on flot nav
* (bluefox) import old settings

### 0.1.1 (2015-07-13)
* (bluefox) fix time format

### 0.1.0 (2015-07-10)
* (bluefox) lines are implemented

### 0.0.2 (2015-07-09)
* (bluefox) implement title and sort points

### 0.0.1 (2015-03-27)
* (bluefox) initial commit

### How to use
- install "web"-adapter and create one instance if not installed.
- Select in settings of "web"-adapter the instance of installed "socket.io"-instance.
- install "flot"-adapter and call
- Go to http://ip:8082/flot/edit.html
