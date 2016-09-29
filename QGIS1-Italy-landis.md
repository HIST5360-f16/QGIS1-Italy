# Italy in QGIS: A Tutorial on Adding Vector Layers
### Author: Whitney.Landis@mavs.uta.edu
## This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial about adding layers](http://programminghistorian.org/lessons/qgis-layers)

1. Make a folder or directory called **Italy** on your computer.
2. Download the following Italy data sets from DIVA-GIS into that directory and unzip them; each should be in its own sub-directory.
	* Find it by [clicking here](http://www.diva-gis.org/gdata)
	* Administrative Areas: ITA_adm
	* Roads: ITA_rds
3. Open QGIS and set up a new project.
4. Set up CRS (Coordinate Reference System) so that the project is using the Monte Mario (Rome) / Italy zone 1 (26591). You select the CRS for the project under the Project Properties.
5. Next we need to build a base map: Open these vectors, then change the way they look using the “properties”:
	* ITA_adm0.shp; change so there is no color fill.
	* ITA_adm1.shp; change so there is no color fill.
	* ITA_roads.shp; change the color and width of the lines so they are easier to see, if needed.

6. Look at the attribute table of ITA_adm1.shp. These show the country’s regions. Note which one of the columns gives the name of the region. Note the name of that column. Close the attribute table. Go into the “properties” for ITA_adm1.shp into “labels”. Change so that your map shows the names of the regions in a large font.
7. Familiarize yourself with the historical context in order to understand what the cartography tells you about Italian history. [Italian Unification](https://en.wikipedia.org/wiki/Italian_unification#The_Second_Italian_Independence_War_of_1859_and_its_aftermath)
8. Open the *1870 Brue Map of Italy.* Import this file as a raster layer in QGIS.
9. Go back to ITA_adm0.shp and ITA+adm1/shp and change the width of the lines so they are visible.
10. In the left-hand “layers” panel, drag the map layer so you can see the parish lines of the historical map.
11. Open the *Charles Scribner’s Sons 1890 Map of Italy.* Import this file as a raster layer in QGIS. Drag it in the “layers” panel just as you did the last map.
12. Go back into the Properties of your various layers. Play with border width and labels, and re-order your layers, to get a feel for the various ways you can manipulate maps in QGIS.
13. Now let's work with georeferencing, and add a preunification map of the Italian states. Download the [Irfanviewer](http://www.irfanview.com/).
14. Go to [Carte](https://www.google.com/search?q=map+of+pre-unification+italy&biw=1920&bih=964&tbm=isch&tbo=u&source=univ&sa=X&ved=0ahUKEwibtcfRqrXPAhWGGR4KHeEqDkYQ7AkILA&dpr=1#imgrc=eyQRnrSyHFHDWM%3A) and save the image as a JPEG.
15. Batch Convert the image through Irfanviewer into a TIF file.
16. Select the "Georeferencer" option through the "Raster" option on the toolbar.
17. Choose several corroborating points from the _Carte_ map and the shapefile. When you are finished, amke sure that you select the option to send to QGIS.
18. You should see the _Carte_ map superimposed over the shapefile. Go to the layer and change the transparency to 35%. This should allow you to easily view the current roads and modern map contrasting through the _Carte_ image. 
19. Smile! You can now look at preunification and postunification political information about Italy underpinned by the hyperaccurate GIS information. Thats pretty cool.
20. Save your work.  Play around with some of the features and see what else you can extrapolate. Close QGIS.
