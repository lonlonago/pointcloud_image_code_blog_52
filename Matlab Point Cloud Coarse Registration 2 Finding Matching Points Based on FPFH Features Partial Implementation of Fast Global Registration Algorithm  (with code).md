#  Function overview 

##  1. Algorithm overview 

   To find matching features between point clouds, most of the algorithm theory comes from the paper: Zhou, Qian-Yi, Jaesik Park, and Vladlen Koltun. "Fast global registration." In European Conference on Computer Vision, pp. 766-782. Springer, Cham, 2016. 

##  2. Main functions 

 Overloaded function 1: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537823
  ```  
   Find matching features between the input matrices of the extracted point cloud features and return their indices in each feature matrix. Overload function 2: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537823
  ```  
   Eliminate fuzzy feature matching based on the spatial relationship information of the point cloud corresponding to the feature matrix. Overload function 3: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537823
  ```  
   Returns the normalized Euclidean distance between matching functions using any combination of input parameters from the previous syntax. Overloaded Function 4: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537823
  ```  
   Specifies the option to use one or more name-value corresponding parameters, in addition to any parameter combinations in the previous syntax. For example, "MatchThresHolding", 0.03 sets the normalized distance threshold for the matching feature to 0.03. 

 input parameter 

 Name-value corresponding parameter 

   Specify optional comma-separated name pairs, value arguments. Name is the parameter name and value is the corresponding value. The name must appear in quotes. You can specify multiple name and value pair arguments as Name1, value 1,., Nmen, ValueN in any order. 

>  Note: If you want to consider spatial relationships, you must match at least three features between the feature matrices. 

 output parameter 

##  3. References 

>  [1] Muja, Marius and David G. Lowe. “Fast Approximate Nearest Neighbors with Automatic Algorithm Configuration.” In Proceedings of the Fourth International Conference on Computer Vision Theory and Applications, 331-40. Lisboa, Portugal: SciTePress - Science and Technology Publications, 2009. https://doi.org/10.5220/0001787803310340. [2] Zhou, Qian-Yi, Jaesik Park, and Vladlen Koltun. “Fast global registration.” In European Conference on Computer Vision, pp. 766-782. Springer, Cham, 2016. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537823
  ```  
#  III. Display of results 

 ![avatar]( e14227dc997f4c90b9cbdd1c205fdbcf.png) 

#  IV. Reference link 

 Matlab Point Cloud Toolbox - pcmatchfeatures 

