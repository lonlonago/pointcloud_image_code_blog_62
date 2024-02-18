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



--------------------------------------------------------------------------------

##  I. Overview of algorithms 

  Compute the connected endpoints around any vertex in the mesh model data. 

###  1. Main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574574281
 ```  
##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574574281
 ```  
##  III. Display of results 

![avatar]( 9168bddbbadf4388bdbf7eb99898a00c.png) 



--------------------------------------------------------------------------------

##  I. Overview 

  Smart pointers, which are widely used in Open3D, are shared_ptr. shared_ptr acts like pointers, but keeps track of how many shared_ptrs together point to an object. This is called reference counting. Once the last such pointer is destroyed, that is, once an object's reference count becomes 0, the object is automatically deleted. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566570
 ```  
##  III. Display of results 

![avatar]( dde7ec89f6f24c2f809857aa1244f71c.png) 



--------------------------------------------------------------------------------

##  Direction towards customization 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555427
 ```  
Function for normal orientation. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555427
 ```  
##  III. Display of results 

![avatar]( aea72b0596ab41569ceb571a39c6dea9.png) 



--------------------------------------------------------------------------------

##  First, towards the camera position 

###  1. Algorithm principle 

   For any point, the normal vector is and the camera position is:, to make the normal vector towards the camera position, simply:  

###  2. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565394
 ```  
Function for normal orientation. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574565394
 ```  
##  III. Display of results 

![avatar]( 65314ca8624f4bc298ad59044c41a13f.png) 



--------------------------------------------------------------------------------

##  Towards the interior of the point cloud 

   As the question, the algorithm is extremely simple, no need to introduce the principle, just look at the code!! 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538041
 ```  
##  III. Display of results 

![avatar]( 562db58e37a947b48a2cfc29a4eb26bc.png) 



--------------------------------------------------------------------------------

##  Towards the outside of the point cloud 

   As the question, the algorithm is extremely simple, no need to introduce the principle, just look at the code!! 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458992
 ```  
##  III. Display of results 

![avatar]( 0fb54b7c77c5467295385b83584bc050.png) 



--------------------------------------------------------------------------------

##  I. Overview 

  The main steps of normal spatial sampling are as follows: 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574516209
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574516209
 ```  
![avatar]( 02e801823a9e4455b27a16fe21c91d0b.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Overview 

  The method of computing the normal vector in this version is to use the matrix factorization method of the Eigen library, and the implementation principle is the same as that of the PCL calculation point cloud normal vector and display. 

###  2. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553684
 ```  
###  3. Algorithm source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553684
 ```  
##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553684
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574553684
 ```  
![avatar]( 5d87bcf6856b4a7d858c70f1b56e6490.png) 



--------------------------------------------------------------------------------

##  I. Overview 

###  1. Algorithm source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524329
 ```  
###  2. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524329
 ```  
  A function that computes vertex normals, usually called before rendering. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574524329
 ```  
##  III. Display of results 

###  1. Before calculation 

![avatar]( bbb162bdab1949879587872a843006b0.jpeg) 

###  2. After calculation 

![avatar]( 7ec63036a02c41908f35dd606dca4632.jpeg) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Algorithm overview 

   Fleishman et al. proposed a grid bilateral filter. The bilateral filter was first applied to grey release images. The algorithm not only considers the distance from the point to the neighborhood point, but also uses the distance along the normal direction as the basis for judgment. In addition, the algorithm has no restrictions on the normal direction. The bilateral filter is applied to the point cloud data. For a certain point in the middle, first use the point within the neighborhood range of the point to calculate the unit normal vector of the point, and then the position of the point is updated by the equation. In the formula, it is the new point after the measurement point has been filtered bilaterally; it is the weight factor of the bilateral filter. In the formula, it is the unit normal vector of the near-neighborhood point of the measurement point; it is the Gaussian kernel function that is the standard deviation, that is, the two Gaussian weights in the point cloud bilateral filtering algorithm. Among them is the influence factor of the distance from the measurement point to its near-neighborhood point on the point, but the influence factor of the distance vector from the measurement point to its near-neighborhood point projected on the normal vector of the point on the measurement point; it is the spatial domain weight, which controls the smoothness degree; it is the feature domain weight, which can capture the change of the normal between neighborhood points, thereby controlling the feature retention degree. 

![avatar]( 20210613083258295.png) 

    As can be seen from Figure 1, the weight of the neighborhood point distance will be balanced by the weight of the normal direction, which is conducive to bringing the target point close to the tangent plane. The normal is obtained by computing the least squares regression plane of the neighborhood points, which is calculated from the average value of the neighborhood points and the covariance matrix.  

###  2. Calculation steps 

Bilateral filtering calculation steps based on normal: input: a certain point, neighborhood radius, two Gaussian weights, output: denoising point 

Therefore, the position of the point cloud after bilateral filtering based on normal will change, and the number of points will remain unchanged. 

###  3. References 

>  [1] Digne J, Franchis C D. The Bilateral Filter for Point Clouds [J]. Image Processing On Line, 2017, 7:278-287. [2] Yuan Zhicong. Research on point cloud registration method based on Harris feature [D]. Donghua University of Technology, 2019. [3] Liu Chuncheng. Column target change detection based on point cloud data [D]. Beijing University of Civil Engineering and Architecture, 2018.p43-44 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574589483
 ```  
##  III. Display of results 

![avatar]( b08adb7e20204623ad43f91f2048ad7a.png) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

##  I. Overview of algorithms 

  The convex hull (convex_hull) is a concept of computational graphics. In two-dimensional space, the convex hull can be regarded as the minimum convex polygon of all points in a point set. At present, there are many C++ implemented two-dimensional convex hull codes on the Internet, but they have not been specifically applied to the extraction of convex polygon boundaries from plane point clouds. Therefore, combined with the existing reference materials and codes on the Internet, I make appropriate modifications to make the two-dimensional convex hull algorithm can be applied to the extraction of convex polygons from plane point clouds. 

###  1. Calculation process 

![avatar]( 616d225abcb84bb092b2a35112b66980.png) 

###  2. Reference link 

[1] 凸包问题的GRAHAM-SCAN解法(附C++代码) [2] Graham Scan算法 [3] C++/Qt：凸包 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574511238
 ```  
##  III. Display of results 

![avatar]( d18de6a3274c42e181f5f40a53626d1b.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Gaussian noise 

  The Gaussian distribution, also known as the normal distribution, is denoted as the parameters of the distribution, which are the expectation and variance of the Gaussian distribution, respectively. When there is a definite value, it is also determined that the distribution, especially when, is the standard normal distribution. The so-called Gaussian noise refers to a type of noise whose probability density function obeys the Gaussian distribution (i.e. normal distribution). Note that in the generation of simulated measurement point clouds, this noise is only equivalent to moving an existing point by one position, rather than adding new points. 

###  2. References 

>  [1] Sun Wenxiao, Wang Jian, Liang Zhouyan, Ma Weili, Chen Zhe. Exact registration of laser point clouds constrained by normal features [J]. Journal of Wuhan University (Information Science Edition), 2020, 45 (07): 988-995. [2] Peng Zhen, Lv Yuanjian, Qu Chao, Zhu Dahu. Point cloud registration based on key point extraction and optimization of iterative closest points [J]. Advances in Laser and Optoelectronics, 2020, 57 (06): 68-79. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574593416
 ```  
##  III. Display of results 

![avatar]( 8ae693fa806c4740a5f7125b4b78daec.png) 

##  IV. Python code 

Open3D point cloud adds Gaussian noise and saves 



--------------------------------------------------------------------------------

##  I. Overview 

  Adding Gaussian noise points along the direction of the point cloud normal vector to the points in the point cloud data. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574571533
 ```  
##  III. Display of results 

![avatar]( c422e18fd6ff409c94084a8fdcf4d7e0.png) 



--------------------------------------------------------------------------------

##  First, uniform distribution 

  In probability theory and statistics, a uniform distribution, also known as a rectangular distribution, is a symmetric probability distribution in which the probability of a distribution at the same length interval is equally likely. The uniform distribution is defined by two parameters, a and b, which are the minimum and maximum values on the number line, usually abbreviated as. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574539336
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574539336
 ```  
![avatar]( 8ad93a7bc96c41cf9a452e61f508ecc8.png) 



--------------------------------------------------------------------------------

AABB bounding box

```
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458726
``` 
OBB bounding box

```
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458726
```


--------------------------------------------------------------------------------

##  I. Overview 

  Directly call the color rendering function in Open3D to attach a color to each point in the point cloud based on the elevation information of the point cloud, and save the color rendering result to a .pcd file. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574562666
 ```  
##  III. Display of results 

![avatar]( 976aebd2024f4dcfbc95d08e2032e44a.png) 



--------------------------------------------------------------------------------

##  I. Overview of algorithms 

  3D Delaunay is a tetrahedral mesh, and a simple implementation of this algorithm is also available in Open3D. 

###  1. Main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538292
 ```  
This function is used to create a three-dimensional Delaunay triangulation, resulting in a tetrahedral mesh. The Qhull library interface is used. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538292
 ```  
##  III. Display of results 

>  Red is the dot in the cloud. 

![avatar]( 42be99a874c74976b9a45210c95d6f5c.png) 



--------------------------------------------------------------------------------

