#  Function overview 

##  1. Algorithm overview 

   Intrinsic shape feature (ISS) is a three-dimensional shape representation method. Feature points of ISS have rich 3d structural variations around them. The method can be used for modeling, visualization and classification of 3D point clouds. To detect ISS feature points in point clouds, its detection function follows the following steps: 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524588
  ```  
   Detects Inherent Shape Feature (ISS) feature points in the input point cloud ptCloud. ISS is a three-dimensional shape representation method for three-dimensional object recognition. ISS feature points are points in their neighborhood that are rich in three-dimensional structural changes. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524588
  ```  
 In addition, the index of the detected ISS feature points is returned. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524588
  ```  
 Specify options using one or more name-value parameters, and any combination of output parameters using the previous syntax. For example, detectISSFeatures (ptCloud, Radius = 0.05) calculates the ISS significance within a 0.05 m radius around each point when identifying feature points. 

##  3. Input and output parameters 

>  The value of NonMaxRadius must be less than or equal to the value of Radius. Otherwise, the function reduces the value of NonMaxRadius to the value of Radius. 

##  4. References 

>  [1] Zhong Y . Intrinsic shape signatures: A shape descriptor for 3D object recognition[C]// IEEE International Conference on Computer Vision Workshops. IEEE, 2010. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524588
  ```  
#  III. Display of results 

 ![avatar]( b3c5056faabe460aa5b48d398a57cd25.png) 

#  Fourth, a warning!!! 

   Copy and paste the code and run it directly. Don't read other content on the blog. If you report an error, you can directly open "Why did I report an error, what kind of garbage code is this"??? detectISSFeatures is a new function in matlab2022a and above, so why do some bosses make mistakes?? Why ask?????  

