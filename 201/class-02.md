# Duckett HTML:

### Chapter 2: Text

**Headings < h# >**: there six heading [ h1-h2-h3…], h1 used for the main headings and the rest go for subheadings. And as the heading number increased its importance is decreased.

**Paragraphs < p>**: to create and write a paragraph.

**Bold < b> & Italic < i>**: to apply one of these two features, just write the text you want to change between the feature tag.

**Superscript < sup>**: used to write characters as superscript. Like “4th”

**Subscript < sub>**: used to write characters as subscript. Like “CO2”

**Line break < br />**: used to start a new line, paragraph, heading

**Horizontal rule < hr />**: used make to make a break (adding horizontal rule), like between two topics

**Semantic Markup**: They are elements used not to change the structure of the web page, but to add 
additional information.

**Strong < strong>**: this element used to indicate the importance of the content

**Emphasis < em>**: indicates a change in the sentence’ meaning and is show in italic.

**Quotations**: 
 -	**Blockquote < blockqoute>**: used for long quotes such as paragraph.
 -	**< q>**: used for short quotes

**Abbreviations < abbr>**: used to inform about the abbreviation and what it stands for. And title attribute is used in the opening tag to show what is stands for.<br>

**Acronyms < acronym>**: used to inform about the acronym and what it stands for.  And title attribute is used in the opening tag to show what is stands for.

**Citations < cite>**: used when referencing for something, such as: to refer to book.

**Definitions < dfn>**: used to indicate a definition for a new term, concept.

**Address < address>**: used to have the contact information about the author.

Changes to Content:
 -	**< ins>**: to show or inform that the content is inserted to a document. And the element is shown underlined.
 -	**< del>**: to show that a text is deleted. And the element is shown as line go through it.
 -	**< s>**: to indicate that something is no more accurate (but not deleted).

 
### Chapter 10: Introducing CSS

+ CSS is used to style the HTML.

Associating style rule with HTML: 
  it has two parts:
   -	Selector: indicate what element is having the style or the rule will applied on.
   -	Declaration: indicates the styling for the element.

+ CSS declarations is made up of two parts: 
  -	Property: show the aspect of the element to change
  -	Value: the setting for the property 

And I can set more than property in one declaration.

+ Steps of linking External CSS:

 - < link >: used to inform the HTML document where to find the CSS file.<br>
 - href: used to appoint the path of CSS file <br>
 - type: used to appoint the type of document being linked to. <br>
 - rel: used to show the type of document being linked to. <br>

*Internal CSS*: 
< style >: element that CSS use it to be included its rules within HTML page.

+ An external CSS style sheet should be used when building a site with more than one.


Types of selectors (p. 238):
 1.	Universal selector * {}: for all elements on the page
 2.	Type selector: it matches the selected element 
 3.	Class selector .classname{}
 4.	Id slecetor #idname{}
 5.	Child selector: target a direct child element of another. li>a {}
 6.	Descendent selector: target a descendent element of a specified element. 
 7.	Adjacent sibling selector: target an element that is the next sibling for another. h1+p {}

# Duckett JS:

### Chapter 2: Basic JavaScript Instructions 

*Script*: is a set of instructions that the computer will follow.

*Statement*: is induvial instruction and it ends with semicolon.

*Comment*: used to add explanations to the code which help you and others to read the code. And there are two types of comment:
 1-	Multi-line comment: add /* in the beginning of the comment and */ at the end 
 2-	Singe line comment: add // and anything follows the two slash will be comment.
 
*Variable*: used to store a set of data inside it, and it should have a name related to its content. **The declaration** of a variable is by **giving it a name**, and to **assign a value** *use the assignment “=” operator*. 

+ Data types: 
 -	Strings
 -	Numbers
 -	Boolean

The variable can have any of the three data types.

+ Rules of naming variable: 

 1-	Must start with letter, dollar sign or underscore <br>
 2-	Can contain letters, dollar sign, numbers or underscore, but no dash (-) or dot (.)<br>
 3-	Cannot use keywords or reserved words <br>
 4-	All variables are case sensitive. Eg.: score & Score are two different variables <br>
 5-	Using a name for the variable that is related to its content <br>
 6-	Use the **camel case method** in naming the variable.


*Array*: is a type of a variable used to store list of values. It is declared like any other variable, but as for assigning the values they should be in square brackets and separated by comma.

e.g: color = [ ‘white’, ‘black’, ‘blue’] => this is called array literal

e.g: color = new Array ( ‘white’, ‘black’, ‘blue’)  this is called array constructor

The values in the array considered as numbers and the numbering of the list start with zero “0”.
To change the value in an array is by specifying the index number of the value.
e.g: colo[ 2] = ‘green’

*Experssions*: 

There are two expressions:

1- Expressions that just assign a value to a variable. <br>
2- Expressions that use two or more values to return a single value.

Operators: they are used to create a single value from one or more values, and they are used in Expression. 

Examples of operators:
 - Assignment operators 
 - Arithmetic operators 
 - String operators
 - Comparison operators
 - Logical operators

+ In Arithmetic operators you need to pay attention to the order if more than one operator is used in one expression.

+ String operators have only one string operator which the + symbol, that used to join the strings.

### Chapter 4: Decisions & Loops

**Decisions**: is the part where it will determine which part of the code will run next.

Two components of a decision:
1-	An expression which will return a value from it.<br>
2-	A conditional statement to inform what to do.

**Comparison Operators**:

 1- **==**: used to compare two values to check if are the same.<br>
 2- **!=**: used to compare two values to check if are not the same.<br>
 3- **===**: used to compare two values & to check if they have the same data type and value as well.<br>
 4- **!==**: used to compare two values & to check if they do not have the same data type and value as well.<br>
 5- **>**: to check if the number on left is greater than the number on the right.<br>
 6- <: to check if the number on left is less than the number on the right.<br> 
 7- **>=**: to check if the number on left is greater equal than the number on the right. <br>
 8- **<=**: to check if the number on left is less than or equal the number on the right.

**Logic Operators**:
Comparison operators **return a values of true or false**. The logic operator allows to compare between the results of the comparison operators.

 1- **&&**: used to test more than one condition. **Both expressions needs to be true to return value as true**, otherwise it will return false.<br>
 2- **||**: used to test at least one condition. **Both expressions needs to be false to return value as false**, otherwise it will return true.<br>
 3- **!**: used to take a single Boolean value and invert its value. It means if the statement was false it will return true, and vice versa


*If statement*: used to check for a condition, if the condition is true the code will run.

*If...else statements*: used to check for a condition. If the condition is true, it will run the code in the first block. But if the condition is false, it will run the code in the second block.
