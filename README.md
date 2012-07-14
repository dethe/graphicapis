# Basic Graphics Techniques across APIs

## New image

## Open image

## Save image

## Rect

Draw a green rectangle 32 x 32 at 200,300

### HTML/CSS

``` html
<div style="width: 32px; height: 32px; position:absolute; 
left: 200px; top: 300px; background-color: green;"></div>
```
    
### SVG

``` svg
<rect width="32px" height="32px" x="200px" y="300px" fill="green" />
```

### Canvas

```javascript
// assumes we have a context
ctx.fillStyle = 'green';
ctx.fillRect(200,300,32,32);
```

### NodeBox

```python
fill(0,1.0, 0);
rect(200,300,32,32);
```

### Python Image Library (PIL)

```python
draw = ImageDraw(im)
draw.rectangle([(200,300),(232,332)],{fill: 'green'})
```

### ImageMagick

Note, for this example, we first create a 500x500 image in memory and fill it with the color skyblue, then we draw the rect, then we save it to the file draw_rect.gif. The middle line is the goal of this exercise.

```bash
convert -size 500x500 xc:skyblue \
-fill green -draw "rectangle 200,300 32,32" \
draw_rect.gif
```

### Processing

```processing
fill(0,255,0);
rect(200,300,32,32);
```

### Raphael

```javascript
paper.rect(200,300,32,32).attr('fill', 'green');
```

### Cocoa

```objective-c
```

## Circle

Draw a red circle centered at 450,250 with a radius of 25

