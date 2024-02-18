##  Vertex clustering 

###  1. Overview 

  Sometimes we want to represent a high-resolution mesh with fewer triangles, but a low-resolution mesh should still be close to a high-resolution mesh. For this Open3d implements many mesh simplification algorithms. The vertex clustering method aggregates all vertices that fall into a voxel of a given size into a single vertex. This method is implemented in SimplifyVertexClustering, the parameter voxel_size defines the size of the voxel mesh, and the contraction defines how the vertices are clustered. There are Average and Quadric ways. 

###  2. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568426
 ```  
The return result of this function can be a non-manifold mesh. 

###  3. Algorithm source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568426
 ```  
##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568426
 ```  
##  III. Display of results 

![avatar]( 492f727230374530a3cf5bd0dc215f92.png) 

 1  1/32  1/16  1/8  

