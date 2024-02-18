#  Function overview 

##  1. Implement the algorithm 

   alphaShape creates an edge interface or three-dimensional volume that can enclose a set of two- or three-dimensional points. You can manipulate alphaShape objects to tighten or loosen a fit that includes these points to create non-convex areas. You can also add or remove points, or hide holes or areas. After creating alphaShape objects, you can perform geometric queries. For example, you can determine whether a point is within a shape, and you can also calculate the number of areas that make up that shape. You can also calculate some useful quantity values, such as area, perimeter, surface area, or volume, as well as draw shapes for visual inspection. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
 Create a 2D alpha shape with points, using the default alpha radius. The default alpha radius will produce the most compact fitted alpha shape, including all points. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
 Using the default alpha radius, create a three-dimensional alpha shape that contains dots. shp represents a polyhedron. A polyhedron has polygonal properties as described earlier, but it does not have isolated faces or dangling edges. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
 Specifies the points, or, in each column of the matrix. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
 Create an alpha shape with an alpha radius of a using any of the parameters in the above syntax. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
 Use one or more Name, Value for additional options specified by the group parameter. For example, you can use'HoleThreshold 'to hide internal holes or voids. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565847
  ```  
#  III. Parameter analysis 

##  input parameter 

 For two-dimensional shapes, the columns represent coordinates and coordinates, respectively. 

 For three-dimensional shapes, the columns represent, coordinates, and coordinates, respectively. 

>  When the extreme value of a is Inf, a convex hull is generated; when it is 0, an empty alpha shape is generated. Data type: double 

##  Name value corresponding parameter 

>  When specifying'HoleThreshold 'and'RegionThreshold', the application of these thresholds depends on the order. The alphaShape fills holes between hidden areas. 

>  When specifying'HoleThreshold 'and'RegionThreshold', the application of these thresholds depends on the order. The alphaShape fills holes between hidden areas. 

#  IV. Display of results 

 ![avatar]( b32ef9975f754724bef96fb7ef105afd.png) 

#  V. Reference links 

 alphaShape 

