
## To view PageSpeed scores:


1. Check out the repository

1. To inspect the site, run a local server

  ```  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080  ```


1. Open a browser and visit localhost:8080

1. Download and install [ngrok](https://ngrok.com/) to make the local server accessible.

  
``` 
  $> cd /path/to/your-project-folder
 
 $> ngrok 8080 ```


1. Copy the public URL ngrok gives you and run it through PageSpeed Insights!


___


### Optimizations performed for Critical Rendering Path for index.html


1.Inlined CSS

1.Moved scripts to end of body

1.Made scripts asynchronous

1. Optimized pizzeria image


___


### Optimizations performed for Framerate for pizza.html


1. Optimized javascript  by managing variables inside for-loop in updatePositions().

1. Further reduced scripting time by using a faster method namely
 ``` javascript
 getElementsByClassName() ```
 instead of

 ``` javascript
 querySelectorAll()
```


1. Cached length of array for use in loops

1. Managing amount of pizzas needed by using screen.width and windows.innerHeight to calculate pizzas based on screen.

1. Removed
``` javascript
style.height
style.width
```
on loading and resized pizza.png to pizza-small.png so pizzas are already small when loaded.




___


### Optimizations performed for Computation Efficiency for pizza.html


1. Optimized resizePizzas() by removing function determingDX() and setting the width of the pizzas to the new width directly in changePizzaSizes()




___



