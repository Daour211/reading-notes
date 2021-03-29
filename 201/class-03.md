# Duckett HTML:

### Chapter 3: Lists 

**Ordered list**: use the < ol> tag to create ordered list and inside it we use the <li> tag to set each item.

**Unordered list**: use the  <ul> tag to create unordered list and inside it we use the <li> tag to set each item.

Definitions lists:
 < dl>: definition list tag used to consist a series of terms and their definitions. And inside it we have < dt> & < dd> tags as pairs.
 < dt>: contain the term that is going to be defined.
 < dd>: contain the definition of the term

**Nested list**: created by adding a list inside an < li> element


### Chapter 13: Boxes

**Box dimensions**: to set the dimension of a box, we use:
 -	Height
 - 	Width

Both of can be specified by pixels or percentages which the most popular units.

Limiting Width: by using
 -	min-width: to the smallest size can be displayed when the window is narrow
 -	max-width: : to the largest size can be displayed when the window is wide

Limiting Height: by using
 -	min-height: to the smallest size can be displayed when the window is narrow
 -	max-height: to the largest size can be displayed when the window is wide

**Overflowing content**: overflow property used to inform the browser how to deal with a content that is larger than the box. And this done using two values:
 1.	overflow: hidden: it hides any extra content that does not fit in the box
 2.	overflow: scroll: it adds scroll bar to show all the missing content that is not shown

Each box has 3 properties can be modified to control its appearance:
 1.	Border: every box has its border, which separate the boxes from each other.
 2.	Margin: it is the space outside the border of the box 
 3.	Padding: it is the space between the border of a box and the element inside it.

*Border width*: used to determine the width of a border. Its values can be as pixels or one the following: 
 -	 thin
 -	medium
 -	thick
e.g: border-width: 4px; 
     border-width: thin

Also I can specify which side of the border I want to edit: top, right, bottom, left.
e.g: border-left-width: thick


*Border Style*: I set the border style
e.g: border-style: solid;
     border style: dotted

*Border Color*: I can set the whole border color or any side I want f the border
e.g: border-color: blue; 
     border-top-color: red; 

Border property **“border”** can be used as shorthand to set the width, style, color in one property.
e.g: border: 4px dotted blue;

**Padding**: I can set the padding I want, between the element and the box. And I can specify a certain side of the element.
e.g: padding:10px;
      padding-top: 4px;

**Margin**: I can set the margin I want, between the boxes. And I can specify a certain side of the element.
e.g: margin:10px;
      margin-top: 4px;


**Centering**: 
-	to center a box 	inside a page (or center it inside the element which sits in), we set the left and right margins to auto. And the width of the box needs to be set or it will take the full width of the page

**Change Inline/Block**: The property “display” allows to turn inline element to block-level element and vice versa. The values of the property:
 -	inline: change the act from block-level element to inline element 
 -	block: change the act from inline element to block-level element
 -	inline-block: change the act from block-level element to inline element, but it keep other features of a block-level element 
 -	none: it hides the element from the page
e.g: display: none;

**Hiding boxes**: using the “visibility” property to hide the boxes from users. This property takes two values: 
 1.	hidden: hide the element
 2.	visible: show the element

**Border Images**: “border-image” property applies an image to the box’s borders. Take the background of an image and cut it to 9 pieces.

The property requires 3 pieces of information:
 1-	URL of the image
 2-	Location (where) of slicing the image
 3-	What to do with straight edges, and there 3 values for this
  -stretch: it stretches the image 
  -repeat: it repeats the image
  -round: like rpeat 

The box must have a border width in order for the image to be shown.

**Box Shadows**: “box-shadow” property used to add drop shadow to a box.  It has 4 values:
 -	Horizontal offset: negative value set the position of the shadow to the left
 -	Vertical offset: negative value set the position of the shadow to the top
 -	Blur distance: if it is removed, the shadow will appear like a solid line like a border
 -	Spread of Shadow:  positive value will make the shadow expand in all directions and vice versa if it is negative.
The “inset” keyword can be used before the four values to create inner shadow 

**Rounded corners**: the “border-radius” property used to make round corners on any box, and its values indicates the size of the radius.
I can specify each corner with different values, and they ordered clock wise.: 
e.g: border-top-right-radius: 2px;
     border-bottom-right-radius: 3px;

I can specify horizontal and vertical parts of the corner to make complex shapes.
e.g: border-top-left-radius: 30px 50px;






# Duckett JS: 

### Chapter 2: Basic JavaScript Instructions

*Array*: is a type of a variable used to store list of values. It is declared like any other variable, but as for assigning the values they should be in square brackets and separated by comma.

e.g: color = [ ‘white’, ‘black’, ‘blue’] => this is called array literal

e.g: color = new Array ( ‘white’, ‘black’, ‘blue’)  this is called array constructor

The values in the array considered as numbers and the numbering of the list start with zero “0”.
To change the value in an array is by specifying the index number of the value.
e.g: colo[ 2] = ‘green’

### Chapter 4: 
Switch: switch statement start with a variable called switch value. And there are cases inside the switch statements, each one indicates a possibility for the switch value and each one has its code, the code will run if value matches the case.

switch (level) { 
case 'One ': 
title= 'Level 1 ' ; 
break; 
case 'Two': 
tit 1 e = ' Level 2 ' ; 
break; 
case ' Three' : 
title = 'Level 3' ; 
break ; 
default : 
title= 'Test';
break;
}
 

**Type coercion**: converting the data type to complete an operation. 

*JS is considered using a weak typing which means the data type for a value can be changed. Other language considered using a strong typing because you must specify what data type for each variable will be.*

*It is more preferable to use strict equal operators because type coercion can lead to unexpected values and cause errors.*

Truthy and Falsy values: 
 -	Falsy values: values treated as they were false.
 -	Truthy values: values treated as they were true
 ![Falsy values](img/Falsyvalues.png)
 ![Truthy values](img/Truthyvalues.png)


CHECKING EQUALITY & EXISTENCE:
*Unary operator*: it returns a result with one operand 

![JS strict equal operator & falsy values](img/JSstrictequaloperator&falsyvalues.png)

**Short circuit values**:
 
 Logical operator always processed from left to right, but they can be stopped as soon as a result is appeared.

 Logical operator can return different values from true or false:
  -	Because they return the value where the processing was stopped
  -	Because the values can be considered as truthy or flasy even though it was not a Boolean 

  ![related to shortcircuit value](img/relatedtoshortcircuitvalue.png)



**Loops**: it checks the condition and if it returns true then the code in the block will run, and it shall repeat the process by checking the condition agian until the returned value if false.

Three types of loops:

- **for**: used to run a code for specific number of times, and the condition usually is a counter.
- **while**: used when you do not know how many times you want to run the code.
- **do while**: it is almost the same as *while loop* but with one difference that it runs the statement inside the curly braces at least once.

*loop counter*: used by the **for loop** as a condition.

The condition of the *for loops* made up of three statements:
 1- Initialization: create and set a variable to 0. 
 2- Condition: used to keep running the loop until it reaches a specified number.
 3- Update: Each time the loop run the statement in the curly braces, it will add one to the counter.
