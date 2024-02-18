##  I. Overview 

  Smart pointers, which are widely used in Open3D, are shared_ptr. shared_ptr acts like pointers, but keeps track of how many shared_ptrs together point to an object. This is called reference counting. Once the last such pointer is destroyed, that is, once an object's reference count becomes 0, the object is automatically deleted. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574566570
 ```  
##  III. Display of results 

![avatar]( dde7ec89f6f24c2f809857aa1244f71c.png) 

