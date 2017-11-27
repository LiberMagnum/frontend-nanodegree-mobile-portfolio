## Website Performance Optimization portfolio project
### My Optimizations
In index.html, I removed the web font and added css directly into the html instead of linking to a stylesheet. I also made the javascript files async and used grunt to resize some of the images. In views/js/main.js, I changed the changePizzaSizes function so that dx and newWidth were determined once outside of the for loop instead of for every single pizza. In updatePositions, I moved scrollTop out of the for loop. I also moved the background pizzas to a new layer in views/css/style.css so that the entire page does not need to be repainted every time the user scrolls.

### How to Run the Application
To run the application, download the repository and open dist/index.html. The src folder contains the original Udacity repository while the dist folder contains my changes to it.

### Grunt
To run Grunt, first, if necessary, install it globally in node.js by typing 
```
npm install -g grunt-cli
```
Then, navigate to the dist folder and install grunt-contrib-clean, grunt-contrib-copy, grunt-mkdir, and grunt-reponsive-images. Finally, type the command 
```
grunt responsive-images
``` 
to run the Gruntfile. 
