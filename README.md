# Mapping_Earthquakes
![EarthquakePageBanner](https://user-images.githubusercontent.com/84881187/132139996-d8d765d3-19a3-40f6-9cea-5cc275fa150a.jpg)


## Project Overview

We were tasked with creating a page that will visually show the difference between the magnitudes of earthquakes all over the world over the last 7 days. We used a URL for GeoJSON earthquake data from the USGS website; and retrieved geographical coordinates and the magnitudes of earth quakes for the last seven days. We then took that data, and displayed it on an interactive map.

## Project Process

 We usedthe JavaScript and D3.js library to retrieve the coordinates and magnitudes of the earthquales from the GeoJSON data. Using resources from the Leaflet library, we plotted the data on a Mapbox map through and API request, and made the visualized earthquake data interactive. 
 
 Using our original project with two different maps and earthquake overlay, we refactored our logic.js file to visualize the earthquake data in relation to tectonic plate locations. We also created a third map that would isolate, and visualize earthquakes with a magnitude greater than 4.5. To make our visualization more readable, we also included a 3rd, dark, map. Please see below for a screenshots of the 3 map styles:
 
 
 **Street Map**
 ![Streets_Page](https://user-images.githubusercontent.com/84881187/132139274-7e9b7d9b-2432-4412-aabb-901933b05b53.PNG)
 
 
 **Satellite Map**
![Satellite_Page](https://user-images.githubusercontent.com/84881187/132139279-b11b946d-0c4b-4543-a7f1-cc0509cb9800.PNG)


**Dark Map**
![Dark_Page](https://user-images.githubusercontent.com/84881187/132139282-12cb58bc-f625-4732-a3fc-a806d5bb8757.PNG)

 
 Using JavaScrip, Leaflet.js, and the GeoJSON data, we added the tectonic plate data to our existing page. We used d3.json() to add the tectonic plate data, added the data using the geoJSON() layer, and set the tectonic plate LineString to stand out on a map. The tectonic plate data was also added as an overlay object option for the dropdown visualization key.

![Menu_Open_All](https://user-images.githubusercontent.com/84881187/132139151-da46bb6f-9f51-41a1-827d-793422d0f5fa.PNG)

![Tectonic_Plates](https://user-images.githubusercontent.com/84881187/132139350-bd48c3f3-b398-40b7-a6c4-286bf83d547e.PNG)

Our tectonic plate overlay is visually represented in all maps and can be removed and/or isolated using our menu. 

**Tectonic Plates removed from map**
![No_Tectonic_Plates](https://user-images.githubusercontent.com/84881187/132139334-a6aa7951-b593-4aac-9c3b-ec4902814813.PNG)


**Tectonic Plates isolated on map**
![Tectonic_Plates](https://user-images.githubusercontent.com/84881187/132139369-e60fb044-2572-478a-af3e-90eed077bc6f.PNG)


 
We also used d3.json() callback to call the major earthquake data. We modified the radius style format to make them more distinct on the map, and added an overlay layer to isolate them visually as well. Please see below for an example screenshot:

![Major_Earthquakes](https://user-images.githubusercontent.com/84881187/132139231-8b6ed59c-aaae-46b1-a652-94e9732361b3.PNG)



Our visualization is not only customizeable, but interactive so that the user can select an earthquake occurrence, and be provided with the Location and Magnitude of the earthquake itself.

![Earthquake_Info](https://user-images.githubusercontent.com/84881187/132139441-4e7dcf51-ee1f-4a8a-8e54-e6968abfc961.PNG)



## Project Summary

Our visualization displays tectonic plate data and their relation to earthquakes around the world over the last 7 days. We also modified the visualization for earthquake magnitudes over a 4.5. The page allows for the user to view all of these objects together, invidiually, or mixed on the map through a menu. The menu also allows the user to use 3 different types of map styles to view the data. Once the desired menu options have been selected, the user can then click on a specific earthquake radius to learn about the location and magnitude of the earthquake. 

Our visualization could be refactored to collect more data from the USGS database. We could include a dropdown to increase and/or decrease the amount of time our data is collected from. We could create a callback to display earthquake data from only the current day, or from the whole year. This would allow for more customized data with a more diverse sampling. I would also go back and reedit the colors, or add a drop down to make the colors more friendly to color-blind users. While our data does a great job creating contrast, we could redit the colors to be just as readable while account for color-blind viewers. We could also add a menu option to switch the color schemes by choice. Our data visualization is customizeable and readable, but can always be improved
