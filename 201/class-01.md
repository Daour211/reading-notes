# Duckett HTML:

### Chapter 1:

The chapter explains about the HTML and that is the structure of the page. There are two main parts of the page:

1.	Head
2.	Body

**Tags “elements”**: 

They are like containers which provide an information about the content that is between the closing and opening tags. 

Types of tags:
  -	Opening tag
  -	Closing tag
  -	Self-closing tag

**Attributes**:

They add information which are additional to the content of an element. They are written in the opening tag and made up of two part that are separated by “=”: 

 -	Name: show the type of the extra information about the element
 -	Value: information about the attribute and it is placed between double quotes

### Chapter :

- **DOCTYPE**: it is a declaration to inform what version of HTML is being used.

- **Comment < !-- comment -- >**: used to add comments to the code and it is no visible to the user.

- **Id attribute**: it is used to distinguish or identify that element from other elements. It starts with a letter or an underscore. Be attention that no two elements on the same have the same value of the id attributes on the same page.

- **Class Attribute**: it is a way to identify several elements on the same page.
Block Elements: They are elements which always start on a new line in the browser window and they are called Block Level. 
Examples of block elements are: < h1 >, < p >, < ul >, and < li >.

- **Inline Elements**: they are elements which continue on the same line as their neighboring elements. 

Examples of inline elements are: < a >, < b >, < em >, and < img >.

- **Grouping Text & Elements in a Block**: *< div >* it creates a group set of elements in one box level.

- **Grouping Text & Elements inline**: *< span >* it used either for

  - Contain a section of text where there is no other element used to differentiate it from its surrounding text.

  - Contain a number of inline elements

And mostly people use < span > so they can control the appearance of the content using CSS.

- **< iframe >**: it is an abbreviation of inline frame, and it is like a small window that appears in your page — and in that window you can see another page. One of the most common uses for iframe is embed a Google Map.

There are a few attributes to know how to use the iframe element: 

 - src
 - height
 - width
 - scrolling
 - frameborder 
 - seamless


**__Information about the page__**:

**< meta >**: an element that include information about the web page and it appears in the <head> element. And it is not visible to the users. Most common attributes used in <meta> element are: name and content.

**Escape Characters**: characters that are reserved in HTML.


### Chapter 17:

Headers & Footers: they are parts of the body and appear on the top < header > and the bottom < footer >.

- **Navigation < nav >**:  an element that is used to navigate in the site through major navigational blocks.

- **Article: < article >** works as a container for any section of the web page and this sections can be syndicated or independent.

- **Aside: < aside >** its usage depends on its location whether its inside the element < article > or not. If it is inside, it contains information related to the article but not for its essential meaning. And if it is outside, acts as container for a content that is related the entire page.

- **Sections**: < section > it classifies related content together, and each section has its own heading. It may have several distinct <article> elements. On the other hand, if there is a long article a <section> element can be used to divide the article.
Also this element it should not be used as a container for an entire page. It is preferable to use <div> element.

- **Headings**: *< hgroup >* it is used for headings and it varies from 1 up to 6 depending on the importance of the subject.

- **Figures < figure> < figcaption>**: it is used to contain any content that is referenced from the main subject of an article.

Examples of usage include: <br>
● Images
● Videos
● Graphs
● Diagrams
● Code samples
● Text that supports the main body of an article

<figcaption> element should always be inside the <figure> element, it provides description of the content of figure element. <br>

**Sectioning elements**: < div > defines a division or a section. <br>

**Linking around block-level elements**: < a > use this tag to link to other pages. <br>

### Chapter 18: 

Helpful questions to build and design the website:

 1-	Who is the Site for?

 The site is created for an audience and it important to understand this target.

 2-	Why People Visit YOUR Website?

 You must know the reason for visiting the website.

 3-	What Your Visitors Are Trying to Achieve?

 This question is to look for the key tasks or the motivation

 4-	What Information Your Visitors Need

 In this step you must provide the visitors with information about the what they are looking for, so they can fulfill their goals.

 5-	How Often People Will Visit Your Site

 This question is a significant one, especially for the sites that needs to be updated frequently.

- **Site Maps**: this is to show the information that are going to be presented in the site pages. 

- **WireFrames**: it is like a sketch that shows the main information in each page.

Another important point is how to deliver the message to the visitors. And by **organizing and prioritizing the information**, the user can understand the order of the page and the importance. Method or techniques used for organizing and prioritizing:

 -	*Visual hierarchy*: it is a way of arranging and showing elements in order of their importance.     Visual contrast between the materials, items is what creates the visual hierarchy.  This can be presented using: images, font size, font color or font style. <br>

 -	*Grouping and similarity*: are ways of organizing the elements of the page to be viewed. Grouping the information that are related to each other make the design easier to understand it. As for the similarity the repetition of some features such as: color. size, font, shape…etc. shows that the elements have the same importance or meaning. <br>

# Duckett JS:

### Chapter 1:

**Script**: is a set of series instructions to fulfill a goal. It is not necessary to run the whole script; it may run only subset of the code.  

Three steps can be helpful to write the instruction: 
 1-	Define the goal
 2-	Design the script 
 3-	Code each step

**Object**: used in programming to represent physical things.

**Properties**: each property has its own name and value.

**Events**: it is like a trigger for a specific action of the code 

**Methods**: it is the way to perform a task through set of instructions (code). It uses the properties of the object.

Two ways to write JS:

 1-	If the user write directly in HTML file, he will write the JS code between the opening and closing tags < script> JS code < /script>
 
 2-	Link the file of JS to the HTML page using the < script> tag and by adding the src attribute to inform about the location of JS file.


