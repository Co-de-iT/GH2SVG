![cover](https://raw.githubusercontent.com/Co-de-iT/GH2SVG/master/media/GH-to-SVG.png)
# GH2SVG  – YOUR GRAPHICS DIRECTLY FROM GRASSHOPPER
A suite of components for saving SVG file directly from your Grasshopper file
  
We all know the value of data in computational design field. We often need to inform our models with several fluxes of information and just as often show those information using dataviz or infoviz graphics. Co-de-iT decides to maximize the workflow speed in Grasshopper and code some components in order to export real-time graphics in SVG format.  
  
SVG is fully compatible with your favorite vector graphics software (Inkscape or Illustrator) and... your browser! Just drag and drop the .svg file in a new Chrome browser tab.  
  
The components are actually released as grasshopper clusters (they are literally syntax parsers that transform GH data in SVG objects syntax) in order to let anyone to implement the components with other features. The SVG code is really easy to understand and code!  
  
In the GH definition you will find these clusters:  

– line SVG  
– polyline SVG  
– polygon SVG  
– circle SVG  
– curve SVG  
– text SVG  
– composer SVG  
  
The dataviz shown in the ‘GH to SVG’ definition is inspired by this [amazing serie of dataviz done by Simon Vorhammer](http://simonvorhammer.de/?portfolio_item=tree-diagram) I found [here](http://www.grasshopper3d.com/photo/hauer-iii-grasshopper-weaving-simon-vorhammer-30/prev?context=user).
  
Instructions:  

– First of all you have to define the background size and color in the composer SVG component.   
– Use all the clusters you need to convert your grasshopper geometries and text to svg syntax.  
– use a merge component to collect all the data you want to export. Remember! the first data in the merge component will be on the bottom and the last one will be in front (as the photoshop layers) so if you want to chance the appearence position on the background of a set of geometries you can chance the position in the merge component.  
– connect the merge component output data to the composer (all the data must be flattened).  
– save your .svg file with the dedicated button in the definition.  
– drag and drop your SVG file into a new Chrome Tab and press F5 to refresh the file after any change you do in GH*.  
     *there are some Chrome extensions that refresh the page after any change of source code but we haven’t tested it until now.  
– or if you prefer open your SVG fle in your preferred graphic software as Inkscape or Illustrator.  
  
This is a raw sketch of an SVG exporter; maybe it will be updated in the future, but as Co-de-iT we ARE **NOT** interested into developing a Grasshopper plugin (we really don’t have time to spend on the manteinance and future upgrades to grasshopper new versions) so feel free to use it, to customize it to your needs (if you want to report us your improvements and share your work with the GH community you are more than welcome) and if someone of you want to use it as base to develop a SVG plugin … feel free to do it (if you want to give us credits for the initial idea it would be great too).
  
Some reference link just in case you want to understand more about SVG syntax and code:
  
. [SVG examples](http://www.w3schools.com/svg/svg_examples.asp)  
. [SVG reference](http://www.w3schools.com/svg/svg_reference.asp)  
  
  
Here below is another example of SVG dataviz created using the GH to SVG definition:
  
![sample graph](https://raw.githubusercontent.com/Co-de-iT/GH2SVG/master/media/Screenshot_4.png)
