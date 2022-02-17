
### Notes

Some of these environments also have a concept of forward, right and up. Here are some of those conventions:

|         | forward | up | right |
|---------|---------|----|-------|
| blender | +y      | +z | +x    |
| unity   | +z      | +y | +x    |
| unreal  | +x      | +z | +y    |

### Colour conventions for axes

Generally the color conventions when denoting axes are:

- ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) `Red - x axis`
- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) `Green - y axis`
- ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) `Blue  - z axis`


### Handedness

This is whether or not the base vectors (axis directions) of the coordinate system follow the [right handed rule](https://mathworld.wolfram.com/Right-HandRule.html), or not.

So taking and open right hand and curling the fingers from x->y should yeild z being in the direction of the thumb. If so, then you have a right handed system, e.g:

```
y  
↑         ↗ x  
|       . 
|     . 
|   . 
| .
+----------→ z  
```

Going from one to the other is simple for a given coordinate, but mathematical operations that have to be performed need to be consitent with the handedness of the coordinate system those points are in. 

For example if you are rotating a vector using a rotation matrix, the same matrix cannot be used on vectors coming from different coordinates systems.


### Coordinate systems of some common graphics programs

#### Open gl
```

            ↑ y       ↗ x
            |       .
            |     . 
            |   . 
            | .
 ←----------+----------→ z
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```
#### 3drepo.io web api

``` 
            ↑ y       ↗ x
            |       . 
            |     . 
            |   . 
            | .
 ←----------+----------→ z
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```

#### Unreal

```
            ↑ z       ↗ x
            |       . 
            |     . 
            |   . 
            | .
 ←----------+----------→ y
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```

#### Direct x

```
            ↑ y       ↗ x
            |       . 
            |     . 
            |   . 
 z          | .
 ←----------+----------→
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```

#### Unity
```
            ↑ y       ↗ x
            |       . 
            |     . 
            |   . 
 z          | .
 ←----------+----------→
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```
#### 3drepo.io web viewer
```
            ↑ z       ↗ x
            |       . 
            |     . 
            |   . 
 y          | .
 ←----------+----------→
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```
#### AutoCAD/Civil3D/Revit (User coordinate system, UCS)
```
            ↑ z       ↗ x
            |       . 
            |     . 
            |   . 
 y          | .
 ←----------+----------→
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```
#### Blender
```
            ↑ z       ↗ x
            |       . 
            |     . 
            |   . 
 y          | .
 ←----------+----------→
          . |
        .   |
      .     |
    .       |
  ↙         ↓
```
