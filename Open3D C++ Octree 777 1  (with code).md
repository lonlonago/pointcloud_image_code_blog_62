##  Octree 

  An octree is a tree data structure in which each internal node has eight sub-nodes. Octrees are commonly used for spatial partitioning of three-dimensional point clouds. The non-empty leaf nodes of an octree contain one or more points that belong to the same spatial subdivision. An octree is a useful description of three-dimensional space that can be used to quickly find nearby points. Open3D's geometric type, Octree, can be used to create, search, and traverse octrees with a user-specified maximum tree depth max_depth. 

##  Second, point cloud construction octree 

###  1. Main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
###  2. Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
###  3. Display of results 

![avatar]( e5a5064c5e9241be92eeab035bd3ae9a.jpeg) 

##  Voxel construction of octree 

###  1. Main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
###  2. Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
###  3. Display of results 

![avatar]( 39d93ad827cf4c8bb92909bad087a82f.png) 

##  Fourth, traverse the octree 

###  1. Main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
The brief DFS traverses the octree from the root, with a callback function calling each node. 

###  2. Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
###  3. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
![avatar]( e5a5064c5e9241be92eeab035bd3ae9a.jpeg) 

##  Find leaf nodes that contain points 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574595967
 ```  
Returns the leaf OctreeNode and octreendeinfo where the query point is located. 

