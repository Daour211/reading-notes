# Duckett HTML:

### Chapter 4: Links

**Writing Links**: I can write a link using the “a” element. I add the link to “href” attribute.

When I link to other websites the value of “href” attribute is known as Absolute URL (the full address), and when I link to other pages on the same site the value is known as Relative URL(no need to specify the domain).

- **When creating a large website**, it is preferred to have the pages of different sections in separated file(directories).

How to write Relative Links: 
![Relative links](/img/Relative-links.png)

**Email links**: to link the email of the user, we add “mailto” to the href attribute.<br>
 e.g: < a href=mailto:jon@example.org ></a>

**Opening links in a new window**:  to open links in a new window we use the “target” attribute, and the value of the attribute is “_blank”.<br>
e.g: < a href=”#” target=”_blank” >< /a>

- To link to a specific part of the page, first you need to identify that element using “id” attribute and the value of the id attribute is used as the value of “href” attribute.
- To link to a specific part of other pages, you need to identify that part using the id attribute , and use the value of  id attribute as the value of “href” attribute, and type prior to that the relative or absolute URL of the page.


### Chapter 15 Layout 

Key concepts in positioning elements:
  -	**Building Block**: Block-level element act as the main the building block of the page layout, while the inline boxes flow between the surrounding text.

  -	**Containing element**: it the outer box that contains another block-level 

  -	**Controlling the position of elements**: in CSS there is Positioning Schemes which allows to control the layout of the page: 

  - **normal flow**: it appears every block-level element on a new line, which will show each item lower than the previous one.

  - **Relative positioning**: this will move the element from the position where it should be in normal flow to where it have been placed.

   - **Absolute positioning**: this will position the element in relation to its containing element.
 
   - **Fixed positioning**: it is a form of absolute positioning which position the element in relation to the browser element. Any element effected by fixed positioning does not affect the position of the surrounding element, and it does not move when the user scroll up/down the page.

   - **Floating element**: it takes out the element out of normal flow and position it to far right or left of its containing box.

- When you move element from overflow, an overlap can occur. The “z-index” property allows to control which box spear on the top.

**Normal Flow**: uses the property "**position: static;**" Each block-level element sits on top of the next one, but It does not need a CSS property to indicate the elements to appear in normal flow.

**Relative positioning**: uses the property” **position: relative;**”. It moves an element in relation to where it would have been in normal flow.

**Absolute positioning**: when the absolute property is applied the box is taken out of normal flow and does not affect the position of the surrounding elements. The property used for it “**position: absolute;**”.

**Fixed positioning**: type of an absolute positioning, which will position the element in relation to the browser window. The property is “**position: fixed;**”

**Overlapping elements**: when overlap occurs, it will show later HTML code sit on the earlier one. To control the overlap, we use the “**z-index**” property and its value is a number, and the larger the number is the closer element will appear on the front.

**Floating Elements**: it uses the “float” property to take an element in normal flow and place it to the far left or right of the containing element.



# Duckett JS:

### Chapter 3: Functions, Methods and Objects

**Functions**: is a series of statements added together set to perform a specific task.

Function declaration: giving a name and writing a statements inside curly braces. It is created from two parts:
 1-	Function keyword “function”.
 2-	Function name.
A
nd after the function name write the curly braces and inside we have the code.<br>
And to execute the statements of the function, we do “calling” the function.

Sometimes an information is needed to be added to the function, and we add this information known as “**parameter**” to perform the task inside the function.<br>

And for calling functions that has parameters, we assign values to the parameters and these called as “**arguments**”.

There are functions which return a value when it is called, and this done by “return” at the end of the function.

Also functions can return more than one value, by using the array.

A function with no name called”**anonyms function**”.

**Immediately invoked function expression (IIFE)**: is functions that has no name and it is excuted as soon as the interpreter across it.<br>
e.g: var area = ( function() {
                       var width = 2;
                       var height =3;
                return width*height;
}())

The final parentheses are the one after the closing curly braces and inform to run the function immediately.<br>

The grouping operators are the opening parentheses before the function word and the last parentheses “*closing one*”, and these used to inform the interpreter to treat the function as expression.

Variable scope: The location where you declare a variable will affect where it can be used in the code. And there are two types:
 1-	Local variable: when the variable is created inside a function called a local variable. And it cannot be accessed outside the function
 2-	Global variable: it is a variable created outside a function and can be used/accessed anywhere in the code.

