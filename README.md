polymer-elements
================

My playground for custom polymer elements.

Created a pie-chart after attending an event in SF

![alt tag](simple-pie-chart/simple-pie-chart.png)

To use it, assuming you have polymer and bower already installed.

Import the platorm and the custom element to a html page:

```html
<script src="platform/platform.js"></script>

<link rel="import" href="simple-pie-chart/simple-pie-chart.html">
```


Add the element to a page and give it some JSON to render the pie:

```html
<simple-pie-chart size="200" lineWidth="2" slices='[{"caption": "Caption1", "color": "red", "slice": 120}, 
                                                    {"caption": "Caption2", "color": "#0000ff", "slice": 45},
                                                    {"caption": "Caption3", "color": "green", "slice": 0.25}]'>
```
                                                      
                                                      
The slice value can be either degrees (0 <slice <= 360) or percentage (0 < slice <= 1.0)
The element (html5 canvas) use radians but I figured percentages or degrees are preferred.



