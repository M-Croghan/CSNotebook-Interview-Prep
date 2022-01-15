# HTML & CSS CONCEPTS & QUESTIONS
### :paintbrush: <span style="color: aqua">What does it mean for a website to be responsive?</span>
Ultimately, a responsive website is one in which the pages and content can adapt to deliver the best experience to the users regardless of what device they're using. Responsive web design allows for websites to adapt and render on all manner of devices and screen sizes.

### :paintbrush: <span style="color: aqua">What is CSS specificity?</span>
Every selector is ranked in a specificity hierarchy. These include:  
- Inline Styles
- IDs
- Classes, Attributes, & Pseudo-Classes
- Elements & Pseudo-Elements  

Specificity is scored whereby the highest ranking style declaration is what wins out in being applied to an element when two or more CSS/style rules are in conflict.

### :paintbrush: <span style="color: aqua">Where would you link a JS file in your HTML?</span>
Scripts can be placed in either the head or the body of an HTML page. A good rule of thumb is to place it toward the bottom of the page, just before the closing ```</body>``` tag. The idea behind this is that scripts can block parallel downloads and so by placing the external file lower in the body, JS parsing and execution doesn't stop the browser from loading the rest of the page.  

If the scripts contain some event-triggered functions or jquery library then we should use them in the head section. If the script writes the content on the page or is not inside a function then it should be placed inside the body section at the bottom. Good rule of thumb:
- Place library scripts or event scripts in the head section.
- Place normal scripts that do not write anything on the page, in the head section until there is any performance issue.
- Place scripts that render something on the web page at the bottom of the body section.

### :paintbrush: <span style="color: aqua">What are the benefits of maintaining an external Javascript file?</span>
* External scripts separate JS code from HTML.  
* Makes code easier to read and maintain.  
* Cached JS files can speed up page loads.

### :paintbrush: <span style="color: aqua">Are the HTML tags and elements the same thing?</span>
No. HTML elements are defined by a starting tag, may contain some content and a closing tag. For example,  
```<h1>```Heading 1```</h1>``` (HTML element).  
```<h1>``` / ```</h1>``` (Represent a starting & closing tag).

### :paintbrush: <span style="color: aqua">What are tags and attributes in HTML?</span>
Tags are the primary component of the HTML that defines how the content will be structured / formatted, whereas Attributes are used along with the HTML tags to define the characteristics of the element. For example, ```<p align=” center”>Interview questions</p>```, in this the ‘align’ is the attribute used which we will align the paragraph to show in the center of the view.

### :paintbrush: <span style="color: aqua">What are void elements in HTML?</span>
HTML elements which do not have closing tags or do not need to be closed are Void elements. For Example ```<br>, <img>, <hr>```, etc.
### :paintbrush: <span style="color: aqua">What is the advantage of collapsing white space?</span>
In HTML, a blank sequence of whitespace characters is treated as a single space character. Because the browser collapses multiple spaces into a single space character and this helps a developer to indent lines of text without worrying about multiple spaces and maintain readability and understandability of HTML codes.

### :paintbrush: <span style="color: aqua">What are HTML Entities?</span>
Because some characters are reserved in HTML, they must be replaced with character entities. Some examples include: '<', '>', '/', '&', etc. To use these characters in our webpage we need to use the character entities called HTML Entities. For example to use the ampersand (&) we must use the entity name: ```&amp;```

### :paintbrush: <span style="color: aqua">What are different types of lists in HTML?</span>
* Ordered ```<ol>``` & Unordered ```<ul>```
    * Within each, individual items are denoted with ```<li>```
### :paintbrush: <span style="color: aqua">What is the 'class' attribute in HTML?</span>
The class attribute is used to specify the class name for an HTML element.  The class attribute can be used on any HTML element, with many having the the same class. It can be used by CSS and JavaScript to perform certain tasks for elements with the specified class name (i.e. styling & functionality).

### :paintbrush: <span style="color: aqua">What is the difference between the ‘id’ attribute and the ‘class’ attribute of HTML elements?</span>
Multiple elements in HTML can have the same class value, whereas a value of id attribute of one element cannot be associated with another HTML element.

### :paintbrush: <span style="color: aqua">Define multipart form data?</span>
Multipart form data is one of the values of the enctype attribute. It is used to send the file data to the server-side for processing. The other valid values of the enctype attribute are text/plain and application/x-www-form-urlencoded.

### :paintbrush: <span style="color: aqua">Describe HTML layout structure.</span>
Every web page has different components to display the intended content and a specific UI. But still, there are few things which are templated and are globally accepted way to structure the web page, such as:
- ```<header>```: Stores the starting information about the web page.
- ```<footer>```: Represents the last section of the page.
- ```<nav>```: The navigation menu of the HTML page.
- ```<article>```: It is a set of information.
- ```<section>```: It is used inside the article block to define the basic structure of a page.
- ```<aside>```: Sidebar content of the page.

### :paintbrush: <span style="color: aqua">How to optimize website assets loading?</span>
To optimize website load time we need to optimize its asset loading and for that:
- ***CDN hosting*** - A CDN or content delivery network is geographically distributed servers to help reduce latency.
- ***File compression*** - This is a method that helps to reduce the size of an asset to reduce the data transfer
- ***File concatenation*** - This reduces the number of HTTP calls
- ***Minify scripts*** - This reduces the overall file size of js and CSS files
- ***Parallel downloads*** - Hosting assets in multiple subdomains can help to bypass the download limit of 6 assets per domain of all modern browsers. This can be configured but most general users never modify these settings.
- ***Lazy Loading*** - Instead of loading all the assets at once, the non-critical assets can be loaded on a need basis.

### :paintbrush: <span style="color: aqua">What are the various formatting tags in HTML?</span>
HTML has various formatting tags:  
```<b>``` - makes text bold  
```<i>``` - makes text italic  
```<em>``` - makes text italic but with added semantics importance  
```<big>``` - increases the font size of the text by one unit  
```<small>``` - decreases the font size of the text by one unit  
```<sub>``` - makes the text a subscript   
```<sup>``` - makes the text a superscript  
```<del>``` - displays as strike out text  
```<strong>``` - marks the text as important  
```<mark>``` - highlights the text  
```<ins>``` - displays as added text  

### :paintbrush: <span style="color: aqua">What are the different kinds of Doctypes available?</span>
The three kinds of Doctypes which are available:
* Strict Doctype 
* Transitional Doctype
* Frameset Doctype

### :paintbrush: <span style="color: aqua">Please explain how to indicate the character set being used by a document in HTML?</span>
The character set is defined in ```<meta>``` tag inside ```<head>``` element.

```<!DOCTYPE html>```  
```<html>```  
``` <head>```  
  ``` <meta charset="UTF-8">```  
   ```...```  
   ```...```  
 ```</head>```  
 ```...```  
```</html>```  

### :paintbrush: <span style="color: aqua">What is the difference between ```<strong>```, ```<b>``` tags and ```<em>```, ```<i>``` tags?</span>
The effect on a normal webpage of the tags ```<strong>```, ```<b>```  and ```<em>```, ```<i>``` is the same. ```<b>``` and ```<i>``` tags stands for bold and italic. These two tags only apply font styling and bold tag adds more ink to the text, these tags don't say anything about the text itself. ```<strong>``` & ```<em>``` tags on the other hand has semantic importance

Whereas, ```<strong>``` and ```<em>``` tags represent that the span of text is of strong importance or more importance and emphatic stress respectively than the rest of the text. These tags have semantic meaning.
### :paintbrush: <span style="color: aqua">What is the significance of ```<head>``` and ```<body>``` tag in HTML?</span>
```<head>``` tag provides the information about the document. It should always be enclosed in the ```<html>``` tag. This tag contains the metadata about the webpage and the tags which are enclosed by head tag like ```<link>```, ```<meta>```, ```<style>```, ```<script>```, etc. are not displayed on the web page. Also, there can be only 1 ```<head>``` tag in the entire Html document and will always be before the ```<body>``` tag.

```<body>``` tag defines the body of the HTML document. It should always be enclosed in the ```<html>``` tag. All the contents which needs to be displayed on the web page like images, text, audio, video, contents, using elements like ```<p>```, ```<img>```, ```<audio>```, ```<heading>```, ```<video>```, ```<div>```, etc. will always be enclosed by the ```<body>``` tag. Also, there can be only 1 body element in an HTML document and will always be after the ```<head>``` tag.

### :paintbrush: <span style="color: aqua">Can we display a web page inside a web page or Is nesting of webpages possible?</span>
Yes, we can display a web page inside another HTML web page. HTML provides a tag ```<iframe>``` using which we can achieve this functionality.

```<iframe src=”url of the web page to embed” />```

### :paintbrush: <span style="color: aqua">How is Cell Padding different from Cell Spacing?</span>
Cell Spacing is the space or gap between two consecutive cells. Whereas, Cell Padding is the space or gap between the text/ content of the cell and the edge / border of the cell.
### :paintbrush: <span style="color: aqua">How can we club two or more rows or columns into a single row or column in an HTML table?</span>
HTML provides two table attributes “rowspan” and “colspan” to make a cell span to multiple rows and columns respectively.
### :paintbrush: <span style="color: aqua">Is it possible to change an inline element into a block level element?</span>
Yes, it is possible using the “display” property with its value as “block”, to change the inline element into a block-level element.
### :paintbrush: <span style="color: aqua">In how many ways can we position an HTML element? Or what are the permissible values of the position attribute?</span>
There are mainly 7 values of position attribute that can be used to position an HTML element:

- static: Default value. Here the element is positioned according to the normal flow of the document.
- absolute: Here the element is positioned relative to its parent element. The final position is determined by the values of left, right, top, bottom.
- fixed: This is similar to absolute except here the elements are positioned relative to the <html> element.
- relative: Here the element is positioned according to the normal flow of the document and positioned relative to its original/ normal position.
- initial: This resets the property to its default value.
- inherit: Here the element inherits or takes the property of its parent.
### :paintbrush: <span style="color: aqua">In how many ways you can display HTML elements?</span>
- inline: Using this we can display any block-level element as an inline element. The height and width attribute values of the element will not affect.
- block: using this, we can display any inline element as a block-level element. 
- inline-block: This property is similar to inline, except by using the display as inline-block, we can actually format the element using height and width values.
- flex: It displays the container and element as a flexible structure. It follows flexbox property.
- inline-flex: It displays the flex container as an inline element while its content follows the flexbox properties.
- grid: It displays the HTML elements as a grid container.
- none: Using this property we can hide the HTML element.
### :paintbrush: <span style="color: aqua">What is the difference between “display: none” and “visibility: hidden”, when used as attributes to the HTML element.</span>
When we use the attribute “visibility: hidden” for an HTML element then that element will be hidden from the webpage but still takes up space. Whereas, if we use the “display: none” attribute for an HTML element then the element will be hidden, and also it won’t take up any space on the webpage.
### :paintbrush: <span style="color: aqua">How to specify the link in HTML and explain the target attribute?</span>
HTML provides a hyperlink - ```<a>``` tag to specify the links in a webpage. The ‘href’ attribute is used to specify the link and the ‘target’ attribute is used to specify, where do we want to open the linked document. The ‘target’ attribute can have the following values:

    _self: This is a default value. It opens the document in the same window or tab as it was clicked.
    _blank: It opens the document in a new window or tab.
    _parent: It opens the document in a parent frame.
    _top: It opens the document in a full-body window.
### :paintbrush: <span style="color: aqua">In how many ways can we specify the CSS styles for the HTML element?</span>
There are three ways in which we can specify the styles for HTML elements:
- ***Inline***: Here we use the ‘style’ attribute inside the HTML element.
- ***Internal***: Here we use the ```<style>``` tag inside the ```<head>``` tag. To apply the style we bind the elements using ‘id’ or ‘class’ attributes.
- ***External***: Here we use the ```<link>``` tag inside ```<head>``` tag to reference the CSS file into our HTML code. Again the binding between elements and styles is done using ‘id’ or ‘class’ attributes.

### :paintbrush: <span style="color: aqua">Difference between link tag ```<link>``` and anchor tag ```<a>```?</span>
The anchor tag ```<a>``` is used to create a hyperlink to another webpage or to a certain part of the webpage and these links are clickable, whereas, link tag ```<link>``` defines a link between a document and an external resource and these are not clickable (i.e. External Stylesheet).
### :paintbrush: <span style="color: aqua">What are forms and how to create forms in HTML?</span>
The HTML form is used to collect the user inputs, it helps organize other elements to be used to take in user input. HTML provides a ```<form>``` tag to create forms. To take input from the user we use the ```<input>``` tag inside the form so that all collected user data can be sent to the server for processing. There are different input types like ‘button’, ‘checkbox’, ‘number’, ‘text’, ‘password’, ‘submit’ etc. [Example can be seen here.](https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_form_submit)

### :paintbrush: <span style="color: aqua">How to handle events in HTML?</span>
HTML allows event trigger actions in browsers using javascript or JQuery. There are a lot of events like ‘onclick’, ‘ondrag’, ‘onchange’, etc.
### :paintbrush: <span style="color: aqua">What are some of the advantages of HTML5 over its previous versions?</span>
- It has Multimedia Support.
- It has the capabilities to store offline data using SQL databases and application cache.
- Javascript can be run in the background.
- HTML5 also allows users to draw various shapes like rectangles, circles, triangles, etc.
- Included new Semantic tags and form control tags.

### :paintbrush: <span style="color: aqua">How can we include audio or video in a webpage?</span>
HTML5 provides two tags: ```<audio>``` and ```<video>``` tags using which we can add the audio or video directly in the webpage.

### :paintbrush: <span style="color: aqua">What is the difference between ```<figure>``` tag and ```<img>``` tag?</span>
The ```<figure>``` tag specifies the self-contained content, like diagrams, images, code snippets, etc. ```<figure>``` tag is used to semantically organize the contents of an image like image, image caption (i.e.```<figcaption>```), etc., whereas the ```<img>``` tag is used to embed the picture in the HTML5 document.

### :paintbrush: <span style="color: aqua">How to specify the metadata in HTML5?</span>
Metadata is used by browsers (how to display content or reload page), search engines (keywords), and other web services, and is never displayed on the actual page. To specify metadata, we can use the ```<meta>``` tag which is a void tag, (i.e. it does not have a closing tag). Some of the attributes used with meta tags are name, content, http-equiv, etc.

### :paintbrush: <span style="color: aqua">What are Semantic Elements?</span>
Semantic elements are those which describe the particular meaning to the browser and the developer. Semantic tags make it clear to the browser what the meaning of a page and its content is. That clarity is also communicated with search engines, ensuring that the right pages are delivered for the right queries. Elements like ```<form>```, ```<table>```, ```<article>```, ```<figure>```, etc., are semantic elements.
### :paintbrush: <span style="color: aqua">Is drag and drop possible using HTML5 and how?</span>
Yes, in HTML5 we can drag and drop an element. This can be achieved using the drag and drop-related events to be used with the element which we want to drag and drop.

### :paintbrush: <span style="color: aqua">What type of audio files can be played using HTML5?</span>
HTML5 supports the following three types of audio file formats:
- Mp3
- WAV
- Ogg


### :paintbrush: <span style="color: aqua">What are the significant goals of the HTML5 specification?</span>
These were the target area of the HTML5 specs:
1. Introduction of new element tags to better structure the web page such as ```<header>``` tag.
2. Forming a standard in cross-browser behavior and support for different devices and platforms.
3. Backward compatible with the older version HTML web pages
4. Introduction of basic interactive elements without the dependency of plugins such as ```<video>``` tag instead of the flash plugin.

### :paintbrush: <span style="color: aqua">Explain the concept of web storage in HTML5.</span>
This web storage helps in storing some of the static data in the local storage of the browser so that we do not need to fetch it from the server every time we need it. There is a size limit based on different browsers. This helps in decreasing the load time and a smooth user experience. There are two types of web storage that are used to store data locally in HTML5:
1. Local Storage - This helps in storing data that will be retained even though the user reopens the browser. It is stored for each webapp on different browsers.
2. Session Storage - This is used for one session only. After the user closes the browser this gets deleted.

### :paintbrush: <span style="color: aqua">Explain HTML5 Graphics.</span>
HTML5 supports two kinds of graphics:
1. Canvas - It is like drawing on a whitepaper or a blank webpage. We can add different graphic designs on web pages with available methods for drawing various geometrical shapes.
2. SVG - Scalable Vector Graphics are used mostly for diagrams or icons. It follows the XML format.

### :paintbrush: <span style="color: aqua">What are the New tags in Media Elements in HTML5?</span>

- ```<audio>```: Used for sounds, audio streams, or music, embed audio content without any additional plug-in.
- ```<video>```:  Used for video streams, embed video content etc.
- ```<source>```: Used for multiple media resources in media elements, such as audio, video, etc.
- ```<embed>```: Used for an external application or embedded content.
- ```<track>```: Used for subtitles in the media elements such as video or audio.

### :paintbrush: <span style="color: aqua">What is SVG?</span>
SVG stands for scalable vector graphics. It’s a text based graphic language which draws images using text, lines, dots etc. This makes it lightweight and renders faster.

### :paintbrush: <span style="color: aqua">What are selectors in CSS?</span>
Selectors help to select an element to which you want to apply a style.

### :paintbrush: <span style="color: aqua">Can you explain CSS box model?</span>
CSS box model is a rectangular space around a HTML element which defines border, padding and margin.
* ***Border***: - This defines the maximum area in which the element will be contained. We can make the border visible, invisible, define height and width etc.
* ***Padding***: - This defines the spacing between border and element.
* ***Margin***: - This defines the spacing between border and any neighboring elements.
### :paintbrush: <span style="color: aqua">What are “web workers”?</span>
Web workers at long last bring multi-threading to JavaScript.

A web worker is a script that runs in the background (i.e., in another thread) without the page needing to wait for it to complete. The user can continue to interact with the page while the web worker runs in the background. Workers utilize thread-like message passing to achieve parallelism.

### :paintbrush: <span style="color: aqua">Can a web page contain multiple ```<header>``` elements? What about ```<footer>``` elements? </span>
Yes to both. In fact, both the ```<header>``` and ```<footer>``` tags are designed to serve their respective purposes in relation to whatever their parent “section” may be. So not only can the page ```<body>``` contain a header and a footer, but so can every ```<article>``` and ```<section>``` element. In fact, a ```<header>``` should be present for all of these, although a ```<footer>``` is not always necessary. 
### :paintbrush: <span style="color: aqua">What is the difference between span and div?</span>
Span and div are both generic HTML elements that group together related parts of a web page. However, they serve different functions. A div element is used for block-level organization and styling of page elements, whereas a span element is used for inline organization and styling.

### :paintbrush: <span style="color: aqua">What’s one main result if you do not specify a doctype in an HTML page?</span>
Not mentioning DOCTYPE will pose a threat to browser compatibility and the use of older versions of HTML. The browser will not support the use of certain new features and tags that come with latest versions of the mark up languages (i.e. HTML5-specific tags will not be interpreted by the browser).