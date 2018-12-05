# OSM public transit

This is a collection of APIs, tools and other cool things that access OpenStreetMap to find or deliver information about public transportation.

## Maps
### [Overpass Line Diagram](http://www.overpass-api.de/public_transport.html) 
Generate horizontal line maps that show stops (including one-ways). Currently a bug exists that may show some stops twice. The API generates an SVG with each map. Here is how the URL structure works: `http://www.overpass-api.de/api/sketch-line?network=NETWORK&ref=LINE&operator=OPERATOR`, where `NETWORK` is a transport network, like the VVO in Germany, `LINE` is a line number, for example "12" for the tram line in Dresden, Germany, and `OPERATOR` is a vehicle operator underneath the network, like DVB. [This](http://www.overpass-api.de/api/sketch-line?network=VVO&ref=12&operator=DVB) would produce the following SVG (converted to PNG to display here):<br><br><img src="https://i.imgur.com/fv1wpaa.png" height="300">
### [Overpass Line Maps](http://www.overpass-api.de/public_transport.html) 
Generate schematic line maps that show stops. Currently a bug exists that may show some stops twice. The API generates an SVG with each map. Here is how the URL structure works:
`http://www.overpass-api.de/api/draw-line?network=NETWORK&ref=LINE`, where `NETWORK` is a transport network, for example the VVO in Germany, and `LINE` is a line number, for example "8" for the tram line in Dresden, Germany. [This](http://www.overpass-api.de/api/draw-line?network=VVO&ref=8) would produce the following SVG (converted to PNG to display here): <br><br><img src="https://i.imgur.com/Wq1mJRe.png" height="300">
