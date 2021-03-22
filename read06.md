## Chapter 10: 

CSS works by HTML rules, and these rules decide how the content of a specific elements appears. 
CSS rule has two parts:

1- Selector: it marks what element that the rule is applied on <br>
2- Declaration: shows how the selector is styled, and is made up of two parts:
  -	Property: it tells about the aspects you want to change about the element  
  -	Value: it shows the settings which are going to be used for the property.

CSS is declared inside the curly brackets (property & value separated by a colon), and more than one property can be declared and they are separated by semi-colon.

**External CSS**:

< link >: used to inform the HTML document where to find the CSS file.<br>
href: used to appoint the path of CSS file <br>
type: used to appoint the type of document being linked to. <br>
rel: used to show the type of document being linked to. <br>

**Internal CSS**: 

< style >: element that CSS use it to be included its rules within HTML page.

An external CSS style sheet should be used when building a site with more than one.


## Cahpter 11:

**Foreground Color**:

*color*: this property allows to select the color inside of text inside the element. And there are three ways to specify the color:
 -	RBG value: specify the color in term of green, red and blue <br>
 -	HEX codes: it is a six-digit color which represent the color by the amount of red, green and blue.
 -	Color names: predefined color names that are known by the browser.

**Background Color**:

The background color is selected by the three ways of the front the foreground color.
Contrast:
  -	Low contrast: it is the hardest to read a text when there is a low contrast between foreground and background color. <br>
  -	High contrast: it is the easiest to read a text when there is a high contrast between foreground and background color. <br> 
  -	Medium contrast: it falls between the high and low contrast.

**Opacity “rgba”**: used to select the opacity of an element and any of its child element. The range of the value between 0.0-1.0.

hsl and hsla: alternative way to choose a color, and its values as follows:

 -	hue: expressed as an angle and its values ranges between 0-360 degrees. <br>
 -	Saturation: expressed as a percentage. <br> 
 -	Lightness: expressed as a percentage, with 0% being white, 50% being normal, and 100% being black. <br>
 -	Alpha: expressed as a number between 0 and 1.0. And the values indicate the transparency.








