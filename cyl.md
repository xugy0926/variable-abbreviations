

## cylinder


cylinder的语义是`圆柱体`，缩写为`cyl`

和大家分享各种形状的英文表达与英英解释

### Types of Shapes
- **square**： a shape with four straight sides that are equal in length and four angles of 90 degrees
- **circle**： a round shape that is like an O
- **semicircle**： half a circle
- **triangle**： a shape with three straight sides and three angles
- **rectangle**： a shape with four straight sides and four angles of 90 degrees
- **oval**： a shape like a circle, but that is longer than it is wide
- **cylinder**： an object in the shape of a tube
- **cube**： a solid object with six equal square sides
- **pyramid**： a shape with a square base and four triangular sides that meet in a point at the top
- **sphere**： a shape like a ball


### 计算圆柱体体积

体积： volume
高：height
半径：radius
直径：diameter

```js
function Cylinder(cyl_height, cyl_diameter) {
  this.cyl_height = cyl_height;
  this.cyl_diameter = cyl_diameter;
}

Cylinder.prototype.Volume = function () {
  var radius = this.cyl_diameter / 2;
  return this.cyl_height * Math.PI * radius * radius;
};

var cyl = new Cylinder(7, 4);
// Volume of the cylinder with four decimal places.
console.log('volume =', cyl.Volume().toFixed(4));
```

上述代码[链接][1]

[1]: https://www.w3resource.com/javascript-exercises/javascript-object-exercise-5.php
