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

