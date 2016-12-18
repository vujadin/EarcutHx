# EarcutHx
Polygon triangulation library for Haxe. Ported from https://github.com/mapbox/earcut

Used in https://github.com/vujadin/BabylonHx

![alt tag](https://github.com/vujadin/EarcutHx/blob/master/bhx.jpg?raw=true)


Usage:
```
// Triangulating a polygon with a hole
var data = Earcut.earcut([0,0, 100,0, 100,100, 0,100,  20,20, 80,20, 80,80, 20,80], [4]);
// data: [3,0,4, 5,4,0, 3,4,7, 5,0,1, 2,3,7, 6,5,1, 2,7,6, 6,1,2]

// Triangulating a polygon with 3d coords
var data = Earcut.earcut([10,0,1, 0,50,2, 60,60,3, 70,10,4], null, 3);
// data: [1,0,3, 3,2,1]
```
