# Image map example
The idea behind an image map is that you should be able to perform different actions depending on where in the image you click. 
# Demo
https://momenmusallam.github.io/image_map_example/
## Getting Started 
### The Image
The image is inserted using the ```<img>``` tag. The only difference from other images is that you must add a ```usemap``` attribute:

    <img src="Burger.jpg"  alt="Burger" usemap="#burger-map">

### Create Image Map
Then, add a <map> element.

The ```<map>``` element is used to create an image map, and is linked to the image by using the required ```name``` attribute: 

    <map name="burger-map">
  
  The ```name``` attribute must have the same value as the ```<img>```'s ```usemap``` attribute .

###  The Areas
  Then, add the clickable areas.

A clickable area is defined using an ```<area>``` element.

### Shape
 You must define the shape of the clickable area, and you can choose one of these values:

```rect``` - defines a rectangular region

```circle``` - defines a circular region

```poly``` - defines a polygonal region

```default``` - defines the entire region

You must also define some coordinates to be able to place the clickable area onto the image. 

in our example we select the ```shape="poly"``` like this:

    <area shape="poly" target="_blank" alt="burger-king" title="Burger King" href="https://www.bk.com/" coords="611,278,572,297,5....." >

the ```coords``` come in pairs, one for the ```x-axis``` and one for the ```y-axis```.So the ```shape="poly"``` contains several coordinate points, which creates a shape formed with straight lines (a polygon).





