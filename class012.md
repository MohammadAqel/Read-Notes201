# CHARTS

*There are three functions that draw rectangles on the canvas:*

1. fillRect(x, y, width, height)_ Draws a filled rectangle.
2. strokeRect(x, y, width, height)_ Draws a rectangular outline.
3. clearRect(x, y, width, height)_ Clears the specified rectangular area, making it fully transparent.

## Drawing paths:
     
1. beginPath: Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. Path methods: Methods to set different paths for objects.
3. closePath: Adds a straight line to the path, going to the start of the current sub-path.
4. stroke: Draws the shape by stroking its outline.
5. fill: Draws a solid shape by filling the path's content area.
   
## Moving the pen:
  
*moveTo(x, y): Moves the pen to the coordinates specified by x and y.*  
  
## Lines: For drawing straight lines
   
*lineTo(x, y) : Draws a line from the current drawing position to the position specified by x and y.*

- **Arcs** : To draw arcs or circles

  - arc(x, y, radius, startAngle, endAngle, anticlockwise) : Draws an arc which is centered at (x, y) position with radius r 
    starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).
  - rcTo(x1, y1, x2, y2, radius) : Draws an arc with the given control points and radius, connected to the previous point by a 
    straight line.
  -  ![EXAMPLE](https://mdn.mozillademos.org/files/204/Canvas_arc.png)
    
 - **Bezier and quadratic curves** : 
    - quadraticCurveTo(cp1x, cp1y, x, y) : Draws a quadratic Bézier curve from the current pen position to the end point
      specified by x and y, using the control point specified by cp1x and cp1y.
    - bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y) : Draws a cubic Bézier curve from the current pen position to the end point 
      specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).
    -  ![EXAMPLE](https://mdn.mozillademos.org/files/223/Canvas_curves.png)
    1. _Quadratic Bezier curves_
     - ![EXAMPLE](https://mdn.mozillademos.org/files/243/Canvas_quadratic.png)
    2. _Cubic Bezier curves_
     - ![EXAMPLE](https://mdn.mozillademos.org/files/207/Canvas_bezier.png)
  
  - **Rectangles** :
     - rect(x, y, width, height) : Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.
     
  - **Making combinations**
   - ![EXAMPLE](https://mdn.mozillademos.org/files/9849/combinations.png)
   
  
  - **Path2D objects** 
    - available in recent versions of browsers, lets you cache or record these drawing commands.
    - Path2D() : The Path2D() constructor returns a newly instantiated Path2D object, optionally with another path as an argument
      (creates a copy), or optionally with a string consisting of SVG path data.
    - ![EXAMPLE](https://mdn.mozillademos.org/files/9851/path2d.png)
    
    ____________________
    
    ## Colors :
     
     - fillStyle = color : Sets the style used when filling shapes.
     - strokeStyle = color : Sets the style for shapes' outlines.
     - fillStyle example : ![EXAMPLE](https://mdn.mozillademos.org/files/5417/Canvas_fillstyle.png)
     -  strokeStyle example : ![EAXMPLE](https://mdn.mozillademos.org/files/253/Canvas_strokestyle.png)
     
     - **Transparency**
       - globalAlpha = transparencyValue : Applies the specified transparency value to all future shapes drawn on the canvas. 
         The value must be between 0.0 (fully transparent) to 1.0 (fully opaque).This value is 1.0 (fully opaque) by default.
       - A globalAlpha example : ![EXAMPLE](https://mdn.mozillademos.org/files/232/Canvas_globalalpha.png)
       - An example using rgba() : ![EXAMPLE](https://mdn.mozillademos.org/files/246/Canvas_rgba.png)
       
    - **Line styles** :
      - lineWidth = value : Sets the width of lines drawn in the future.
      - lineCap = type : Sets the appearance of the ends of lines.
      - lineJoin = type : Sets the appearance of the "corners" where lines meet.
      - miterLimit = value : Establishes a limit on the miter when two lines join at a sharp angle, to let you control 
        how thick the junction becomes.
      - getLineDash() : Returns the current line dash pattern array containing an even number of non-negative numbers.
      - setLineDash(segments) : Sets the current line dash pattern.
      - lineDashOffset = value : Specifies where to start a dash array on a line.
      - A lineWidth example : ![EXAMPLE](https://mdn.mozillademos.org/files/239/Canvas_linewidth.png)
      - A lineCap example : ![EXAMPLE](https://mdn.mozillademos.org/files/236/Canvas_linecap.png)
        - butt : The ends of lines are squared off at the endpoints.
        - round : The ends of lines are rounded.
        - square : The ends of lines are squared off by adding a box with an equal width and half the height of the line's thickness.
      - A lineJoin example : ![example](https://mdn.mozillademos.org/files/237/Canvas_linejoin.png)
        - round : Rounds off the corners of a shape by filling an additional sector of disc centered at the common endpoint of
         connected segments.The radius for these rounded corners is equal to half the line width.
        - bevel : Fills an additional triangular area between the common endpoint of connected segments, and the separate outside
        rectangular corners of each segment.
        - miter : Connected segments are joined by extending their outside edges to connect at a single point, with the effect of
         filling an additional lozenge-shaped area. This setting is effected by the miterLimit property which is explained below.
         
       - A demo of the miterLimit property : ![example](https://mdn.mozillademos.org/files/240/Canvas_miterlimit.png)
       - Using line dashes : The setLineDash method and the lineDashOffset property specify the dash pattern for lines
        - ![example](https://mdn.mozillademos.org/files/9853/marching-ants.png)
       - A createLinearGradient example : ![example](https://mdn.mozillademos.org/files/235/Canvas_lineargradient.png)
       -  createRadialGradient example : ![example](https://mdn.mozillademos.org/files/244/Canvas_radialgradient.png)
       
       - **Patterns** :
         - repeat : Tiles the image in both vertical and horizontal directions.
         - repeat-x : Tiles the image horizontally but not vertically.
         - repeat-y : Tiles the image vertically but not horizontally.
         - no-repeat : Doesn't tile the image. It's used only once.
         - A createPattern example : ![example](https://mdn.mozillademos.org/files/222/Canvas_createpattern.png)
         
      - **Shadows** :
        - shadowOffsetX = float : Indicates the horizontal distance the shadow should extend from the object. 
          This value isn't affected by the transformation matrix. The default is 0.
        - shadowOffsetY = float : Indicates the vertical distance the shadow should extend from the object.
        This value isn't affected by the transformation matrix. The default is 0.
        - shadowBlur = float : Indicates the size of the blurring effect; this value doesn't correspond to a number
          of pixels and is not affected by the current transformation matrix. The default value is 0.
        - shadowColor = color : A standard CSS color value indicating the color of the shadow effect; by default,
          it is fully-transparent black.
        - A shadowed text example : ![example](https://mdn.mozillademos.org/files/2505/shadowed-string.png)
     
     - **Canvas fill rules**
        - Two values are possible:

           1. "nonzero": The non-zero winding rule, which is the default rule.
           2. "evenodd": The even-odd winding rule.
           
         - EXAMPLE : ![example](https://mdn.mozillademos.org/files/9855/fill-rule.png)
         
         ______________________________
   
  ## Drawing text : 
    
    - fillText(text, x, y [, maxWidth]) : Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
    - strokeText(text, x, y [, maxWidth]) : Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
    
    
    - **Styling text** :
      - font = value : The current text style being used when drawing text. This string uses the same syntax as the CSS font property.
        The default font is 10px sans-serif.
      - textAlign = value : Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
      - textBaseline = value : Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom.
        The default value is alphabetic.
      - direction = value : Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
  
  
   - **Advanced text measurements**
     - measureText() : Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn
       in the current text style.