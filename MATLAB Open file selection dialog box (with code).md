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

