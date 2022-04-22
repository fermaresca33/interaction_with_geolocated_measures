# Interaction, filtering and working with geolocated measures

## Brief Description

This projects aims to manage geolocated data (measurements points or any similar type of usefull information), to filter and interact with it by using simple Python code.

You can follow the "" notebook and be able to play with the information as much as you want.

In this case I decided to try the meteority dataset. So after unzip, load, and some dataframe cleaning; you would see something similar to the following image:

<p align="center">
  <img src="./documentation_files/initial_geo.jpg">
</p>

Once you set "your spot" and a radius to take into consideration, the next geoDataFrames will be generated:

<p align="center">
  <img src="./documentation_files/poin_circle.jpg">
</p>

The next step involves filtering all the meteorites locations based on your selected area. For this the best approach I found was to do an Spatial Join (or sjoin). After you run the respective chunk of code you will see something similar to the following image:

<p align="center">
  <img src="./documentation_files/within_points.jpg">
</p>

After this point you have full control of the data and the area to focus at. You can combine or add more info, make a better way of showing the results or evn storing the geolocated data.

As a last step I considered adding a geopandas to kml code. It's nothing fancy but can help you to have a better way of interacting with the info. Google Earth tends to be very powerfull in managing this kind of information.

Run the code and get a direct download/open link:

<p align="center">
  <img src="./documentation_files/kml_link.jpg">
</p>

You should si something like the following:

<p align="center">
  <img src="./documentation_files/kml_google_earth.jpg">
</p>

You can play with the points stile, size, the table info and much more aspects of the kml.
