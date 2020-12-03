# IMPLEMENTATION
## SOFTWARE IMPLEMENTATION
### 1)Detecting Traffic- open map.html(enter google api key in the code to run)
We leverage the Google Java Script Api to obtain the real time traffic conditions of a certain area which is displayed as traffic layers on google maps. The traffic layer is mainly in three colours-red for heavy traffic, orange/yellow for average and green for low traffic.

![traffic](trafficlayers.png)

### 2)Controlling the movement of median- open colourdetection.ipynb
After getting the live traffic data we make use of OpenCV library on Python to detect the colours/Jam Factor/ Traffic Density  of each road. 
If  there is traffic density/ Jam factor variance on the road in opposite directions and the switch percentage gain is within the range set for the road,  then Smart Median switch is activated. (Eg :  If red and green colours are detected on the same road then the median is made to move towards the green side. If both directions are of same colour then no change required).

![road](road.png)    ![colours](detectedcolours.png)
