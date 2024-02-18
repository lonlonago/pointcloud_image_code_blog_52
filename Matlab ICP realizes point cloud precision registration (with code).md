#  Function overview 

##  1. Implement the algorithm 

   The ICP-related algorithms implemented in the Matlab point cloud toolbox are: point-to-point ICP (pointToPoint ICP), point-to-surface ICP (pointToPlane ICP) and Trimmed ICP. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574584420
  ```  
   The registration of point cloud is realized based on iterative closest point ICP algorithm, and the output is the transformation matrix of registration. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574584420
  ```  
 While outputting the transformation matrix, return the transformed point cloud registered with the fixed point cloud. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574584420
  ```  
 Returns the root mean square error of the point cloud registration. 

>  The'InlierRatio 'attribute corresponds to the Trimmed ICP in PCL. 

##  3. References 

>  [1] Chen, Y. and G. Medioni. “Object Modelling by Registration of Multiple Range Images.” Image Vision Computing. Butterworth-Heinemann . Vol. 10, Issue 3, April 1992, pp. 145-155. [2] Besl, Paul J., N. D. McKay. “A Method for Registration of 3-D Shapes.” IEEE Transactions on Pattern Analysis and Machine Intelligence. Los Alamitos, CA: IEEE Computer Society. Vol. 14, Issue 2, 1992, pp. 239-256. [3] Chetverikov D , Svirko D , Stepanov D , et al. The Trimmed Iterative Closest Point Algorithm[C]// International Conference on Pattern Recognition. IEEE, 2002. 

#  Code implementation 

 pointToPoint ICP 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574584420
  ```  
 pointToPlane ICP 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574584420
  ```  
#  III. Display of results 

 ![avatar]( 20210606071748242.png) 

#  IV. Reference link 

 [1] 使用matlab实现点云匹配（ICP算法） 

