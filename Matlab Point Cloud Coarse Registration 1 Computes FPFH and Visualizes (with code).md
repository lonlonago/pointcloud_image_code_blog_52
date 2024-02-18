#  Function overview 

##  1. Algorithm overview 

   The fast point feature histogram (FPFH) descriptor is extracted from the point cloud, and the detailed calculation method is shown in the reference. 

##  2. References 

>  [1] Rusu, Radu Bogdan, Nico Blodow, and Michael Beetz. "Fast point feature histograms (FPFH) for 3D registration." In 2009 IEEE International Conference on Robotics and Automation, pp. 3212-3217. IEEE, 2009. [2] Han Yifei, Yang Ziqian, Zheng Fu, Wang Yanqiu, Sun Zhibin. Improved point cloud registration algorithm based on FPFH and normal vector [J/OL]. Semiconductor optoelectronics: 1-6 [2021-08-26]. https://doi.org/10.16818/j.issn1001-5868.2021.04.001. 

##  3. Main functions 

 Overloaded function 1: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
   Extract the FPFH descriptor for each valid point in the input point cloud object. The function returns the descriptor in the form of a matrix, where is the number of valid points in the input point cloud. Overload function 2: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
   Extracts the FPFH descriptor of the valid point at the given index. Overloaded function 3: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
   Extracts the FPFH descriptor of the valid point at the specified two-dimensional index of the input organized point cloud ptCloudIn. Specifies the row index and column index of the point as row and column, respectively. Overload function 4: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
   Returns the index of the valid point in the point cloud where the FPFH descriptor has been extracted. Overload function 5: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
   In addition to the parameter combinations in the previous syntax, one or more name-values are used to specify options for parameters. Extraction of descriptors can take the KNN search method, the radius search method, or a combination of the two. The extractFPFHFeatures function extracts descriptors by default using the KNN search method. The user can select the extraction method by name-value on the parameter. For example, 'NumNeighbors', 8 selects the KNN search method to extract the descriptor and sets the maximum number of neighbors to be considered in the k-nearest neighbor (KNN) search method to 8. Enter parameters 

 Name-value corresponding parameter 

>  Note: If you specify values for the "NumNeighbors" and "Radius" name-value pair parameters, the extractFPFHFeatures function will perform a KNN search method and then select only collections within the given radius. If you specify larger values for "NumNeighbors" and "Radius", the memory footprint and computation time increase. 

 output parameter 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562826
  ```  
#  III. Display of results 

>  The code selected two points to output the FPFH, so here is a quick point feature histogram of the two points. 

 ![avatar]( 1631bcf01fc445af9e36368a16c9a4a1.png) 

#  IV. Reference link 

 Matlab Point Cloud Toolbox - extractFPFHFeatures 

