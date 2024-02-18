#  Function overview 

##  1. Algorithm overview 

   The basic idea of the NDT algorithm is to construct the normal distribution of multi-latitude variables. If the transformation parameters are the best match of the two point clouds, the probability density of the transformation points is the largest. Therefore, the optimization method is used to obtain the transformation parameters that make the sum of the probability densities the largest. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459146
  ```  
   The registration of point cloud is realized based on NDT algorithm, and the output is the transformation matrix of registration. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459146
  ```  
 While outputting the transformation matrix, return the transformed point cloud registered with the fixed point cloud. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459146
  ```  
 Returns the root mean square error of the point cloud registration. 

##  3. References 

>  [1] Biber, P., and W. Straßer. “The Normal Distributions Transform: A New Approach to Laser Scan Matching.” Proceedings of IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). Las Vegas, NV. Vol. 3, November 2003, pp. 2743–2748. [2] Magnusson, M. “The Three-Dimensional Normal-Distributions Transform — an Efficient Representation for Registration, Surface Analysis, and Loop Detection.” Ph.D. Thesis. Örebro University, Örebro, Sweden, 2013. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459146
  ```  
#  III. Display of results 

 ![avatar]( 20210606074031787.png) 

#  IV. Reference link 

 Matlab Point Cloud Toolbox - Register two point clouds using NDT algorithm 

