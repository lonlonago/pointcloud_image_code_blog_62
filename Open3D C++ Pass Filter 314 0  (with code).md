##  First, the principle of the algorithm 

   The function of the pass filter is to filter out the points whose values are not within the given range in the direction of the specified dimension. The implementation principle is as follows: First, specify a dimension and the range under that dimension. Secondly, traverse each point in the point cloud to determine whether the value of the point on the specified dimension is within the range. Delete the points whose values are not within the range. Finally, the traversal is completed, and the remaining points form the filtered point cloud. The pass filter is simple and efficient, suitable for operations such as eliminating background. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574537341
 ```  
##  III. Display of results 

###  1. Primitive point cloud 

![avatar]( a3bac2a833604c5fb4cf0ffaa01b543a.png) 

###  2. Filtering results 

![avatar]( cdbd3f030cbc4ae786770298ba40ba4f.png) 

