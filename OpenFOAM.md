Courier new: Linux commands  
**Courier new bold**: directories  
*Courier new italic*: human readable files or ascii files  
**Arial bold font**: variables, function names, classes, statements and so on  

---  

$$\frac{\partial T}{\partial t}$$   
```c++
solve
(
	fvm::ddt(T)
  + fvm::div(phi,T)
  - fvm::laplacian(nu,T)
    ==
    0
);
```
