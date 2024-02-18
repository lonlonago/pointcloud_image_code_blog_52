#  Function overview 

##  1. Definition of Gaussian noise 

   The Gaussian distribution, also known as the normal distribution, is denoted as the parameters of the distribution, which are the expectation and variance of the Gaussian distribution, respectively. When there is a definite value, it is also determined that the distribution, especially when, is the standard normal distribution. The so-called Gaussian noise refers to a type of noise whose probability density function obeys the Gaussian distribution (i.e. normal distribution). Note that in the generation of simulated measurement point clouds, this noise is only equivalent to moving an existing point by one position, rather than adding new points. 

##  2. Matlab Gaussian distribution function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574583833
  ```  
 Generate random numbers from a normal distribution with the mean parameter mu and the standard deviation parameter sigma. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574583833
  ```  
 Generates an array of normal random numbers, where sz1,..., szN indicates the size of each dimension. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574583833
  ```  
 Generates an array of normal random numbers, where the vector sz specifies the size of size. 

##  3. References 

>  [1] Sun Wenxiao, Wang Jian, Liang Zhouyan, Ma Weili, Chen Zhe. Exact registration of laser point clouds constrained by normal features [J]. Journal of Wuhan University (Information Science Edition), 2020, 45 (07): 988-995. [2] Peng Zhen, Lv Yuanjian, Qu Chao, Zhu Dahu. Point cloud registration based on key point extraction and optimization of iterative closest points [J]. Advances in Laser and Optoelectronics, 2020, 57 (06): 68-79. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574583833
  ```  
#  III. Display of results 

 ![avatar]( 685c8d4eaaa84da3a005f4a3ac98e021.png) 

#  IV. Relevant links 

 [1] normrnd——正态随机数 [2] C++代码：PCL 点云添加高斯噪声并保存 [3] python代码：Open3D 点云添加高斯噪声并保存 

