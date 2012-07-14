# Basic Graphics Techniques across APIs

## Draw a green rectangle 32 x 32 at 200,300

### HTML/CSS

``` html
<div style="width: 32px; height: 32px; position:absolute; left: 200px; top: 300px; background-color: green;"></div>
```
    
### SVG

``` svg
<rect width="32px" height="32px" x="200px" y="300px" fill="green" />
```

### Canvas

``` javascript
// assumes we have a context
ctx.fillStyle = 'green';
ctx.fillRect(200,300,32,32);
```

### NodeBox

``` python
fill(0,1.0, 0);
rect(200,300,32,32);
```

### Python Image Library (PIL)

``` python

```

### ImageMagick (Node wrapper)

``` javascript

```

### Processing


### Raphael