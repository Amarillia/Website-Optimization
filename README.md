Website Performance Optimization portfolio project

Getting Started: Download the contents as a zip file and run it in your local browser.

Page load speed optimization

The images were rescaled and optimized to the final layout dimensions.

For the critical above-the-fold content styles, I inlined them and applied them to the bottom of the document.
Below I've included the site to where I found the Google Developer suggested method.

Defer alternative media CSS: Although the print stylesheets are small, they were deliberately chosen not to be served inline in HTML documents due to at least three different pages using it.
*All CSS and JS files were minified to ensure faster downloading. The original files are still present in their respective directories, without the .min in their filenames.
I optimized the Frame rate through Google Developer Tools.

Unnecessary JS operations were pulled out of for loops where possible, in views/js/main.js.
Unnecessary formatting removed from views/js/main.js to the bottom of the html style section.

The scroll events were 'debounced' to split the animations and only reflow/repaint when needed. References https://developers.google.com/speed/pagespeed/insights/ https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery http://www.html5rocks.com/en/tutorials/speed/animations/
