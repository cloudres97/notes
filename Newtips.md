#### 7/24/2021 (*The first day of Tokyo Olympic*)  
1. open the new page in `edge`: <kbd>Ctrl</kbd>+<kbd>T</kbd>    
2. close the page: <kbd>Ctrl</kbd>+<kbd>W</kbd>  
3. switch the page: <kbd>Ctrl</kbd>+<kbd>num</kbd>  
4. search the content selected with `Bing`: <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>E</kbd>  
5. open the files with preferred application in terminal: `$ xdg-open filename`
    - website using: `$ xdg-open https://github.com`
6. aliase 别名
7. compulsory 必修

#### 7/25/2021 (*Typhoon In-fa in ShangHai*)
1. Directory Organization  
```
$WM_PROJECT_DIR ($HOME/OpenFOAM/OpenFOAM-n)
    -Allwmake: 
    -application: (aliase app)
        -solvers
        -test
        -utilities
    -bin: (shell scripts, such as paraFoam)
    -doc: (documentation)
    -etc: (environment files, global instructions, templates)
    -platforms: (binaries and libraries generated from compiling the src files)
    -src: (aliase src) (the source code)
    -tutorials: (aliase tut) (example cases)
    -wmake:
    -COPYING
    -README.org
```
2. Directives set: 指令集
3. save *log* files: `$> blockMesh | tee log.blockMesh`

#### 7/26/2021 (*Still in the dormitory*)
1. `Gnuplot`
    - `gnuplot> set logscale y`: set log scale in the y axis
    - `gnuplot> plot 'logs/p_0' using 1:2 with lines`: plot 'p_0' using columns 1 and 2 with lines
    - `gnuplot> reset`: reset the scales
    - `gnuplot> exit`: exit 
2. `foamClean`
    - `$> foamCleanTutorials`: Mesh/Solution/parallel
    - `$> foamCleanPolyMesh`: Only Mesh
    - `$> foamListTimes -rm`: Solutions
    - `$> foamListTimes -rm -processor`: Solutions in the **processorN** directories
3. Variables in **transportProperties** file
    - *rho* density
    - *nu* kinematic viscosity
    - *mu* dynamic viscosity``
    - *g* gravity
4. vertice: 顶点
5. macro syntax: 宏语法
6. be of paramount important: 至关重要
7. tricky: 棘手
8. **Boundary** types
    |boundary|0/U|0/p|
    |:-:|:-:|:-:|
    |patch|-|-|
    |wall|fixedValue|zeroGradient|
    |movingWall<br>fixedWalls<br>frontAndBack|movingWall<br>fixedWalls<br>frontAndBack|movingWall<br>fixedWalls<br>frontAndBack|
9. Line break in table(html): `<br>`
10. entry: 条目
11. **banana method**: use a dummy word, OpenFOAM will list the available options
12. interpolation: 插值
13. notation: 符号、注释、表示法
14. The type of the field variable(in the header):
    - scalar: `class volScalarField;`
    - vector: `class volVectorField;`
    - tensor: `class volTensorField;`

#### 7/29/2021 
1. curly braces: 大括号
2. Inline calculations:
```
X=10.0;
Y=3.0;
Z #calc "$X*$Y-12.0";
```
3. loop: 循环
4. serial: 串行
5. prompt: 提示(符)
6. identical: 相同

#### 7/30/2021
1. perturbation: 摄动
2. trigger: 触发
3. interpret: 解释
4. divergence: 发散
5. *adjustTimeStep* is only present in **PIMPLE**
6. blend: 混合
7. compressible solvers use absolute pressure

#### 7/31/2021 (*Mount Fuji*)
1. preliminary: 初步
2. overlapping: 重叠
3. fillet: 倒角
4. flange: 法兰
5. skewness: 倾斜
6. deviation: 偏差
7. strive: 努力

#### 8/1/2021
1. Mesh types  

|tetrahedron|四面体|
|:-:|:-:|
|pyramid|四棱锥|
|hexahedron|六面体|
|prism|棱柱|
|polyhedron|多面体|
|quadrilateral|四边形|
|triangular|三角形|

2. metric: 指标
3. diagnose: 诊断
4. orthogonality: 正交性
5. validity: 有效性

#### 8/2/2021
1. for instance: 例如

#### 8/3/2021
1. intersect: 相交
2. *resolveFeatureAngle*  
<img src="https://github.com/cloudres97/PictureSources/blob/main/ResolveFeatureAngle.png?raw=true" width="60%">  

3. digit: 数字  
4. uncheck: 取消勾选  
5. portable: 便携的  
6. bus: 总线  
7. `$> paraFoam -builtin`: post-process the decomposed case directly  

#### 8/4/2021
1. probes: 探针
2. derive: 派生
3. obliged: 强制、有义务的
4. drawback: 缺点

#### 8/7/2021
1. overhead: 开销
2. substitute: 代入
3. sparse: 稀疏
4. dramatically: 大幅
5. hybrid: 混合
6. marginally: 稍微

#### 8/8/2021
1. Set **nCorrectors** > 3 in PISO/PIMPLE if **CFL** is much higher than 1
2. under-relaxation factor: 亚松弛因子
3. monolithic: 整体的
4. Physically speaking, *symmetry* is equivalent to slip wall
5. discharge: 释放

#### 8/15/2021
1. `$> df -hl`: FileSystem ***Ubuntu***
2. Differences from OF versions  
```
FatalErrorIn
   (
        "Foam::sixDoFRigidMotionConstraints::axis::read"
        "("
             "constant dictionary& sDoFRBMCDict"
        ")"
   )
```

```
FatalErrorInFunction
```
3. sixDoFRigidBodyMotionSolver  
`rhoname` -> `rho`
4. 
