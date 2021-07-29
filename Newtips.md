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
    - *mu* dynamic viscosity
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
1. 
