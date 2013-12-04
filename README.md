## SupplyCache
SupplyCache is a web application that helps communities locate resources after a disaster occurs. It maps resources available by residents and the areas affected by a disaster. User input can be via text message or web form. An archived events page builds data visualization for post-disaster analysis. SupplyCache uses Python, Flask, SQLAlchemy, Jinja, JavaScript (Heatmap, Rickshaw), HTML/CSS, Leaflet API, Twilio API, CloudMade API.

### Map
###### Leaflet, OpenStreetMap, CloudMade, Heatmap, MarkerClustering
[Leaflet](http://leafletjs.com/) is an open source JavaScript library for maps: the map data is from [OpenStreetMap](http://www.openstreetmap.org/), an open source map created by communities with an emphasis on local knowledge, and map tiles (style or imagery) are from [CloudMade](http://cloudmade.com/). The heatmap layer uses [heatmap.js](http://www.patrick-wied.at/static/heatmapjs/) and is integrated into my project to display areas affected by a disaster. For example, the redder the area, the more severe the situation. The marker clustering function uses the [Marker Clustering plugin](https://github.com/Leaflet/Leaflet.markercluster) made for Leaflet.

### Data visualiztion
###### Rickshaw
Archived events are accessed via a login due to the sensitivity of the information provided. Once logged in, users will see a line graph that displays supply trends over time for the selected disaster or event. The graph uses [Rickshaw JS](http://code.shutterstock.com/rickshaw/), which is a JavaScript graphing toolkit built on D3. In addition, beneath the graph is a table that summarizes the collected data.

### Database
###### Python, SQLAlchemy
User input is stored into the database with Python, Flask, and SQLAlchemy. The database has also been seeded using Python. The database is used to populate the map, graphs, and tables.

### Web Framework & User Interface
###### Flask, JavaScript, jQuery, HTML/CSS

![Main page](/screenshots/sc-img1.jpg)

![Archive page](/screenshots/sc-img3.jpg)

![About page](/screenshots/sc-img2.jpg)