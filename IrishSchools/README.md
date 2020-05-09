**IRISH SCHOOLS EXPLORER: Information Visualisation: VEGALITE**

**TECHNOLOGY USED:** Vegalite

**AIM:** Interactive Dashboard style visualisation to enable analysis and exploration of Ireland’s primary schools. 

![image](https://user-images.githubusercontent.com/38240162/81474466-860d6680-91fd-11ea-8d97-c0262781bc72.png)


**DATASET:** Irish Primary Schools 

The Irish Primary Schools dataset consists of the details for every primary school in Ireland.

*The dataset consists of:*
	
  1. Roll_No: A unique number associated with the primary school.
  2. Address: The location of the priamry school.
  3. County: The county in which the primary school is located.
  4. Male: Number of male students in the primary school.
  5. Female: Number of female students in the primary school.
  6. Long: The longitude of the primary school loccation.
  7. Lat: The latitude of the primary school loccation.
  8. xcoord: The x coordinates of the school location.
  9. ycoord: The y coordinates of the school location.
  10. Total: Total number of students in the primary school and so on.


*Visualisation 1:*

1. With the help of topojson type of data, a geoshaped map is built initially and on top of it, a point map is layered over with the latitude and longitude given. 

2. Every point represents an Irish school. The point map is further differentiated based on the Sex field (Boys, Girls and Mixed). Lastly the size of every point is mapped to the discretized value of range.


*Visualisation 2:*

1. A layered bar graph with count of the field Roll Number(uniquely identifies the primary school) on the y axis and the Total number of students(field Total) on the x axis is generated.


*Visualisation 3:*

1. A stacked bar graph with County on the y axis and the count of schools on x axis is created. 

2. A color sequence is defined with Boys at first, then for the Girls and lastly for the Mixed gender. 

3. Once all the static visualizations are ready, they are concatenated vertically(point map and layered bar graph) and horizontally ((point map and layered bar graph) and stacked bar graph.) The structure becomes ready.


*Interactive Dashboard:*

*First interaction on point map:*

1. A selection filter named as sexSelection is defined which when clicked single on the field Sex, will display the output of that corresponding category only. 

2. The filter is then bind with the legend and resolved globally. 

*Second interaction on the layered bar graph:*

1. A brush selection named as brush_drag is created of interval type, so that you can select the number of students on the graph. 

*Third interaction on the stacked bar graph:* 

1. A selection filter named as countySelection is defined which selected multiple Counties will display the output of those selected Counties, resolved globally. 


Lastly, all the filters are applied to all three visualizations and an interactive dashboard is ready to visualize.


[![Watch the video](https://github.com/ktyagi12/Information_Visualizations/blob/master/IrishSchools/output/IrishSchools.gif)



[Click here for the code](https://github.com/ktyagi12/Information_Visualizations/tree/master/IrishSchools/code)

[Click here for the output](https://github.com/ktyagi12/Information_Visualizations/tree/master/IrishSchools/output)
