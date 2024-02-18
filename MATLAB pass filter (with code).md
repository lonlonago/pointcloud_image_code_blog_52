#  First, the principle of the algorithm 

##  1. Algorithm overview 

    The function of pass filtering is to filter out the points whose values are not within the given range in the specified dimensional direction. 

##  2. Implementation process 

    First, specify a dimension and the range under that dimension. Secondly, traverse each point in the point cloud to determine whether the value of the point in the specified dimension is within the range. Delete the points that are not within the range. Finally, at the end of the traversal, the remaining points form the filtered point cloud. The pass filter is simple and efficient, suitable for operations such as removing background. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574542962
  ```  
#  III. Display of results 

##  1. X-field filtering 

 ![avatar]( bc01156ec4a74c24884c43252b46f11e.png) 

##  2. Y-field filtering 

 ![avatar]( e7001c39a78c453f819ea83fa49cbd13.png) 

##  3. Z-field filtering 

 ![avatar]( e969c0904cb94f6fbf0e26aa2ed9b71c.png) 

