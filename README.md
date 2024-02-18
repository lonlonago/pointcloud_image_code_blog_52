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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Preface 

   The on-board mobile measurement system can quickly, dynamically and efficiently obtain the three-dimensional point cloud of the road surface and the ground objects on both sides. However, during the vehicle driving process, the obtained point cloud has a certain slope compared with the real scene due to the deceleration belt, road surface damage, unevenness, and bumps. The tripod of the ground 3D laser scanner sinks due to factors such as loose soil at the position of the station, which leads to the deviation of the obtained point cloud from the real scene in the horizontal plane direction, which is not conducive to the high-precision fusion of multi-station data based on four parameters in the later stage. Therefore, horizontal calibration is required. 

##  2. Calibration steps 

##  3. References 

>  [1]张振华. 基于激光点云数据的障碍物检测算法研究[D].山东大学,2020. [2] Dimitrievski, Martin, David Van Hamme, Peter Veelaert, and Wilfried Philips. “Robust Matching of Occupancy Maps for Odometry in Autonomous Vehicles.” In Proceedings of the 11th Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications, 626–33. Rome, Italy: SCITEPRESS - Science and Technology Publications, 2016. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095745211
  ```  
#  III. Display of results 

 ![avatar]( ac6d5cc7161e474bbc84a5409348c812.png) 



--------------------------------------------------------------------------------

#  First, reverse 

    For a matrix, the matrix is invertible if there exists a matrix of the same size so that (where, is the identity matrix). The matrix is called the inverse matrix of. Performs a decomposition of the input matrix (if the input matrix is a Hermitian matrix, the decomposition is performed). It then uses the result to form a system of linear equations, which is solved as the inverse of the matrix. For sparse inputs, a sparse identity matrix is created and backslashes are used, i.e. X\ speye (size (X)). It is rarely necessary to construct an explicit inverse matrix for a certain matrix. When solving a system of linear equations, it is often used incorrectly. One of the ways to solve this equation is to use. In terms of execution time and numerical accuracy, a better approach is to use the matrix backslash operator, i.e. x = A\ b. This is solved using Gaussian elimination without explicitly constructing the inverse matrix. 

##  1. Main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
     Compute the inverse of the square matrix. 

#  Code example 

##  1. Inverse matrix 

    Compute the inverse of a 3x3 matrix. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
    Check the results. Ideally, the identity matrix will be generated. Since inv performs matrix inversion using floating-point computation, in practice Y * X is close to but not exactly equal to the identity matrix eye (size (X)). 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
##  2. Solving linear equations 

    See why solving a system of linear equations by inverting the matrix using inv (A) * b is not as straightforward as using the backslash operator (i.e. x = A\ b). 

 Create a random matrix A of order 500 with condition cond (A) of 1e10 and norm norm (A) of 1. The exact solution x is a random vector of length 500 with b = A * x on the right side. Therefore, the system of linear equations does not set conditions correctly but is consistent. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Solve the linear equations A * x = b by inverting the coefficient matrix A. Use tic and toc to obtain time information. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 T = 0.3760 Find the calculated absolute error and residual. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Now, use the backslash operator\ to solve the same set of linear equations. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
 Calculation result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586992
  ```  
    The backslash method is faster, and the residuals are reduced by orders of magnitude. The fact that both err_inv and err_bs are orders of 1e-6 directly reflects the condition number of the matrix. The behavior of this example is very common. Using A\ b (instead of inv (A) * b) is two to three times faster, and generates residuals (relative to data magnitude) based on computer accuracy. 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  First, non-uniform sampling 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452149
  ```  
 Uses a non-uniform voxel filter to return a downsampled point cloud. This method selects a random point from each box. If no normals are provided in the input point cloud, this method will automatically populate the Normal property in the ptCloudOut output. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452149
  ```  
#  III. Display of results 

##  1. Primitive point cloud 

 ![avatar]( bc98734bfcd944be9f17c586ae813e3b.png) 

##  2. Sampling results 

 ![avatar]( 3ff27c174e974cb7a842ac559f466432.png) 

#  IV. Reference link 

 Matlab point cloud tool - pcdownsample 



--------------------------------------------------------------------------------

#  First, the main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   Opens a modal dialog box that lists the files in the current folder. Here the user can select or enter a name for the file. If the file exists and is valid, uigetfile will return the file name when the user clicks on Open. If the user clicks on the Cancel or Window Close button (X), uigetfile will return 0. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   When the user clicks Open, [file, path] = uigetfile will return the name and path of the file. If the user clicks the Cancel or Window Close button (X), uigetfile will return 0 for both output parameters. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   When the user clicks Open, [file, path, indx] = uigetfile returns the index of the filter selected in the dialog box. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   Specify a file extension by which to filter the files displayed in the dialog box. You can use this syntax in conjunction with any of the output parameters in the above syntax. Typically, only files with matching file extensions are displayed. On some platforms, uigetfile also displays files that do not match the filter, but whose filenames are grayed out. If the filter is missing or empty, uigetfile uses a default list of file types (for example, all MATLAB ® files). 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   Specify the dialog box title. To filter using the default file filter, but to specify a custom title, you need to use empty quotes as the filter value. For example: file = uigetfile (',' Select a File ') 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   Specifies the default file name for the filename field or for the default folder that the dialog box opens. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
   Specifies whether the user can select multiple files. Setting mode to'on 'will allow multiple selection. Default setting is'off'. 

>  Note: The visual characteristics of a dialog box depend on the operating system on which the code is running. For example, some operating systems do not display the title bar in the dialog box. If you pass the dialog box title to the uigetfile function, those operating systems do not display the title. 

#  Code example 

##  1. Display the full file path 

   Displays the full file path of the file selected in the dialog box. Use the disp and fullfile functions to add descriptive text and concatenate the path and file output values. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( c480341dcf664155a435e15f828933d7.png) 

##  2. Display filter index selection 

   Displays the index of the selected filter and associated descriptive text in a command-line window. Use the num2str function to convert the numeric filter index value (indx) to a character array. This makes the index value a valid input to the disp function. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( ff6e97522f904c059d196305ae81fa32.png) 

##  3. Filter files by extension 

   By specifying '* .m' as the filter input parameter, only files with the .m extension are displayed in the dialog box. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 65892087fa064bf88db772462945ff46.png) 

##  4. Specify filter list and dialog box title 

   Creates a list of file extensions to display in the File Filter drop-down list. Pass filter input arguments as a character vector cell array, separated by semicolons. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 5fe422b1eaf44ac8a846ddd371ae024d.png) 

##  5. Specify filters and filter descriptions 

   Creates a list of file name extensions and provides instructions for them by passing the filter input parameter as a character vector cell array. The first column of the cell array contains the file name extension, and the second column contains custom instructions for the file type. This example also associates multiple file types with the'MATLAB Files' and'Models' instructions. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 6fc9f82d1de54312984dafb680dde01e.png) 

##  6. Specify the default file name 

   To display a default filename in the Filename field when the dialog box opens, pass this filename as the defname input parameter. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 7a5b78e5578e4591b38364b6625a11fd.png) 

##  7. Specify the default path and file 

   To display the default filename under the default path in the Filename field when the dialog box opens, pass the full filename as the filter input parameter. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 1170e9a4b5ee4d218209cd918923baca.png) 

##  8. Specify filters and default folders 

   Creates a list of file extensions by passing the filter input parameter as a character vector cell array. Specifies the folder the dialog box opens. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 30302eaf288f49a88ad552de8e04da3f.png) 

##  9. Enable multi-selection 

   Setting the'Multiselect 'option to'on' enables multi-file selection. Users can select multiple files by holding down the Shift or Ctrl keys and clicking on the file name. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590423
  ```  
 ![avatar]( 72ac387bd2b14e57851dd134f45a6942.png) 

#  III. Parameter analysis 

##  1. Input parameters 

 1, filter - file filter 

 ![avatar]( 48033b9250cb458ea691c00473d887b0.png) 

   File filter, specified as a character vector, a character vector cell array, or a string array. The following table lists the types of input that can be passed to the filter parameter and the corresponding behavior of the dialog box. 2. Title - dialog box title 

 ![avatar]( 9b8c886aab8e4303bc6ff233e30d25ff.png) 

 3. Default value of defname - "file name" field 4. Mode - multi-select mode 

   Multi-select mode, specified as'on 'or'off'. If multi-select mode is turned off, the user can select only one file. If multi-select mode is turned on, the user can select multiple files. If the user selects multiple files, they must be in the same folder; otherwise MATLAB will display a warning dialog box. Microsoft ® Windows libraries can span multiple folders. 

##  2. Output parameters 

 ![avatar]( d42ec1af7ce64297ad776cc314d17526.png) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. OBB bounding box 

   OBB (Oriented Bounding Box) is essentially a cuboid that is closest to the object, but the cuboid can be rotated arbitrarily according to the first moment of the object. OBB bounding boxes and AABBs are closer to the object and can significantly reduce the number of enclosures. 

>  Quote from: Baidu Encyclopedia 

##  2. The implementation process 

>  PCL - Minimum Bounding Box 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535654
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574535654
  ```  
 ![avatar]( a54e01e063964afc9297e45863656a49.png) 

#  IV. Reference link 

 [1] PCL ——最小包围盒 [2] matlab 点云配准——三维变换 [3] matlab 点云配准——点云变换 [4] matlab 点云可视化(4)——可视化点云包围框 [5] matlab svd奇异值分解 

#  Warning!!! 

   The rigid3d function is a new function in matlab 2020a and above, so why do some bosses make mistakes?? Why ask??????  



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

##  I. Overview of algorithms 

##  1. Evenly distributed 

   In probability theory and statistics, a uniform distribution, also known as a rectangular distribution, is a symmetric probability distribution in which the probability of a distribution at the same length interval is equally likely. The uniform distribution is defined by two parameters, a and b, which are the minimum and maximum values on the number line, usually abbreviated as. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452434
  ```  
   Returns a random number evenly distributed within the interval (0, 1). 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452434
  ```  
   Returns an n × n matrix of random numbers. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452434
  ```  
   Returns a sz1 ×... × szN array of random numbers, where sz1,..., szN indicates the size of each dimension. For example: rand (3,4) returns a 3 × 4 matrix. In general, N random numbers within the interval (a, b) can be generated using the formula r = a + (b-a). * rand (N, 1). 

##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452434
  ```  
##  III. Display of results 

 ![avatar]( e726e2163ec44f01bc4e2d2effcb5013.png) 

##  IV. Reference link 

 Uniformly distributed random number 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Calculation steps 

 ![avatar]( 5d77abb370174f96aca47ebfb24e143d.png) 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574579031
  ```  
#  III. Display of results 

     The red is the point cloud before filtering, and the green is the point cloud after filtering. The data and parameters are from IPOL Journal · Image Processing On Line.  



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  Box filtering 

##  1. Algorithm overview 

    Given the maximum value of the box coordinates, extract the points within the box. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567657
  ```  
 Returns the points in the region of interest (ROI) in the input point cloud. The points in the specified ROI are obtained using a KD tree-based search algorithm. 

#  Code example 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567657
  ```  
#  III. Display of results 

 ![avatar]( 6305f8ae7e8a422494ced3172c9d9a64.png) 

#  IV. Relevant links 

 Matlab Point Cloud Toolbox - Select points in point cloud 



--------------------------------------------------------------------------------

#  First, the main function 

 ![avatar]( 212660a770714628a1e512baa83018c1.png) 

   The function of MATLAB to build Delaunay triangulation is: delaunayTriangulation, the three-dimensional point that this function needs to enter is double type, and the default storage format of point cloud in pcd format is float, so float needs to be converted to doiuble type. For detailed usage of delaunayTriangulation function, just enter: help delaunayTriangulation in the matlab command line window to view. Since matlab is a non-open source software, the algorithm is only used for simulation experiments and does not go into depth. 

#  Code example 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519909
  ```  
#  III. Display of results 

 ![avatar]( 7bd215d446454455baa722d023623204.png) 

#  IV. The official website 

 delaunayTriangulation 



--------------------------------------------------------------------------------

#  I. Overview 

##  1. Algorithm overview 

   Bsxfun: Apply element-by-element operations to two arrays (enable implicit expansion) 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555249
  ```  
 Applies the per-element binary operation specified by the function handle fun to arrays A and B. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555249
  ```  
#  III. Display of results 

>  The red is the original point cloud, and the green is the decentred point cloud. 

 ![avatar]( e892b69bae764fd1853891d134e2de63.png) 

#  IV. Reference link 

 Binary singleton expansion function for gpuArray 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  Function overview 

##  1. Algorithm overview 

   Visualize the correspondence between matching point pairs. 

##  2. Main functions 

 Overloaded function 1: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538500
  ```  
   Displays the point clouds ptCloud 1 and ptCloud 2 and their matching feature points, matching PtCloud 1 and matedPtCloud 2. The colors of the graph are encoded by the point clouds, and each point cloud is connected to a corresponding point in the other point cloud by a line. Overload Function 2: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538500
  ```  
   Displays the point cloud segments, Segment 1 and Segment 2, and displays their corresponding centroids in the centroids properties of Feature 1 and Feature 2. The graphics are color-coded and the corresponding centroids are connected by a line. Overload Function 3: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538500
  ```  
   In addition, an AXIS object is returned using the input parameters in the previous syntax. Overload function 4: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538500
  ```  
   In addition to any parameter combination in the above syntax, specify the option to use one or more name-value pairs for parameters. For example: 'Method', 'montage' 

 input parameter 

 Name-value corresponding parameter 

 output parameter 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538500
  ```  
#  III. Display of results 

 ![avatar]( caac18182710412f8455fbdeab2ec8b9.png) 

>  The matching features and point clouds are color-coded to enhance the visualization: Magenta - the source point cloud. Green - the target point cloud. Red circle - the matching point in the source point cloud. Blue asterisk - the matching point in the target point cloud. Yellow - the connection between the matching point pairs. 

#  IV. Reference link 

 Matlab Point Cloud Toolbox - pcshowMatchedFeatures 



--------------------------------------------------------------------------------

