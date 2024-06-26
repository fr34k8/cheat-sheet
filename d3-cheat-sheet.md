# D3 cheat sheet
* [d3 documentation](https://d3-wiki.readthedocs.io/)

## alternatives
* https://konvajs.org/
  + vectors
  + events
* https://p5js.org/
  + vectors
  + events
* https://vectorjs.org/
  + vectors
  + svg elements 
* https://g.js.org/
  + vectors
  - no events
* https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API
  - too cumbersome
* https://github.com/pixijs/pixijs
  * games oriented


## Examples
* [my own examples](https://github.com/cherkavi/javascripting/tree/master/d3)
* [galery with examples](https://github.com/d3/d3/wiki/Gallery)
* [d3 extension plottable](https://github.com/palantir/plottable) with [plottable examples](http://plottablejs.org/examples/)
* [d3 scale](https://github.com/d3/d3-scale)

## logging
```js
      function log(sel,msg) {
         console.log(msg,sel);
      }


    svg
      .append("text")
      .attr("x", 0)
      .attr("y", -20)
      .attr("class", "svg_diagram_title")
      .text(title)
      .call(log,title)
      ;

```

## Issues
###  diagram not showing
```
if you don't see any images - check your selector, 
D3 will not complain about 'target element not found '!!!!
```
SOLUTION: fast and small example
```
<html lang="en">
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
  <script src="d3.v5.js"></script>
</head>
<body>
  <svg id="dataviz_area" height=200 width=450></svg>
  <script>
    // MUST BE DECLARED AFTER TARGET ELEMENT DECLARATION
    d3.select("#dataviz_area").append("div").html("hello")
  </script>
</body>
</html>
```
