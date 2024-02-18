#  I. Overview 

   The boundary of a group of points in two or three-dimensional space 

##  1. Main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 Returns a single index vector of points representing a compatible two-dimensional boundary surrounding the points that form the boundary. Unlike the convex hull, the boundary can contract inward to enclose the points. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 Returns a triangulation of a single compatible three-dimensional boundary representing the bounding point. Each row of is a triangle defined as a point index. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 Specifies the points, or, in each column of the matrix. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 Specify a shrinkage factor in conjunction with the above syntax. Is a scalar between 0 and 1. Setting, to 0 generates a convex hull, and setting, to 1 generates a compact boundary surrounding these points. The default shrinkage factor is 0.5. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 Also returns a scalar, which is the boundary surrounding the area (two-dimensional) or volume (three-dimensional). 

#  Code example 

##  1. The boundary of a two-dimensional point cloud 

 1. Use the default shrinkage factor to calculate the boundaries surrounding these points 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 2. Use a shrinkage factor of 0.1 to create a new boundary surrounding these points 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
##  2. Results display 

 ![avatar]( 77a2e47c8a2740bfb27b99e20a16248d.png) 

 1. Use the default shrinkage factor to calculate the boundary surrounding these points 2. Use the shrinkage factor 0.1 to create a new boundary surrounding these points  

##  3. The boundary of a three-dimensional point cloud 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 ![avatar]( 9efe845793d44bc8ad0365312171cf12.png) 

##  4. Shrinkage factor effect on three-dimensional boundaries 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 ![avatar]( 61922dece255471fb3b4daa5bafdcbd9.png) 

##  5. The volume of the three-dimensional boundary 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
 ![avatar]( 81a0774e88fc4263af598ca42d292589.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577573
  ```  
#  III. Parameter analysis 

##  input parameter 

 S = 0 corresponds to the convex hull of these points. 

 S = 1 corresponds to the closest single region boundary surrounding these points. 

 The default contraction factor is 0.5. Specifying a larger or smaller contraction factor tightens or loosens the boundaries including these points accordingly. 

 Example: k = boundary (x, y, 0.76) specifies a shrinkage factor of 0.76 and produces a more compact boundary than the default. 

##  output parameter 

 For a two-dimensional problem, it is a column vector composed of point indices that represent a sequence of points enclosing a boundary (polygon). 

 - For a three-dimensional problem, is a triangulation matrix of size mtri × 3, where mtri is the number of triangular faces on the boundary. Each row of defines a triangle according to the point index, and these triangles together form a bounded polyhedron. V - The area or volume enclosed by the boundary, returned in scalar form. 

 For a two-dimensional problem, it is the boundary, the area enclosed. 

 For a three-dimensional problem, it is the boundary, the volume enclosed. 

#  III. Reference link 

 boundary 

