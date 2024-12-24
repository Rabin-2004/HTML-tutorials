# What is HTML?
- HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on.

- Note: Documentation is in codes. The comments in codes explain neccesary topics


# Nesting Elements
- Elements can be placed within other elements. This is called nesting. For eg:
`<p>My cat is <strong>very</strong> grumpy.</p>`

- Here the `<strong>` tag is nested inside the `<p>` tag.

- In the above example we opened `<p>` first followed by `<strong>` but when closing we closed `<p /strong>` first followed by `</p>` tag. This is the proper way of nesting html elements


# Void elements
- Not all elements require an opening and closing tags. Sometimes, some elements typically which are used to insert something into the document take only one tag. Such elements are called void elements. 
Example: `<img>`, `<br>`, `<hr>`, `<input>`, `<meta>`

- For void elements, the syntax example: `<img src= "heading and meta tags/apple.jpg" />` is valid  but considered unnecessary in HTML file. You can omit the `/` in html but is necessary when you want your tag to be valid in xml.


# Attributes
- Elements can also have attributes. Attributes look like this: `<div classs='demo'> HELLO </div>`. Here the `<div>` element takes `class` attribute that specifies the class this element belongs to.

- An attribute should have: a space between element name and the attribute name followed by an equal to sign.

- The attribute value should be wrapped with an opening and closing quotes.


## Boolean Attributes
- Sometimes an attribute can be without any value. Such attributes are called boolean attributes.

- When a boolean attribute is written without a value, or with any value, even like "false", the boolean attribute is always set to true. Otherwise, if the attribute is not written in an HTML tag, the attribute is set to false.

- For example, consider the disabled attribute, which you can assign to form input elements.
`<input type ='text' disabled >` or `<input type ='text' disabled= 'disabled'>` both have the same effect.


# Omitting quotes around attribute values
- Lets take an example below `<a href=https://www.mozilla.org/>favorite website</a>`.
- The above code is perfectly valid as the `<a>` has only one attribute `href`.

- Again lets take an example: `<a href=https://www.mozilla.org/ title=The Mozilla homepage>favorite website</a>`
- The above example is understood by browser. The `href` will be understood correctly but the `title `attribute will be misunderstood as `title = The` and `Mozilla` and `homepage` will be taken as two Boolean attibutes.

- Always enclose attributes with quotes. This will avoid all the problems.


# Single or double quotes?
- Both are valid and just a preference of styles. Just don't mix them like: single quote as opening quote and double as closing for the same attribute.

- To use quotes inside other quotes use `&quot;` character refrence or ` `` ` backtick quotes.


# Whitespaces in html
- No matter how many whitespaces are used in HTML the browser will always reduce it to one whitespace. The white spaces are only used for readability purposes.

- If you want to use whitespaces, the text inside the `<pre> </pre>` tag will have its whitespaces preserved. Additionally CSS `style ='white-space` will allow to use white-space.

- Additionally, character refrences like `&nbsp; &thinsp; ` also allow whitespaces.

# Character references
- In HTML, the characters <, >, ", ', and & are special characters. They are parts of the HTML syntax itself. These characters will be interpreted as codes in HTML. So, to use these characters we use special codes which represent each of these following symbols which are called character references.

- This document includes the list of all character references <a href ='https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references'> Wikipedia-characterRefrences </a>


# HTML comments
- HTML includes a mechanism to use comments. Browers will exclude comments making them invisible to the user. The purpose of comment is to include notes to explain the code or logic
-- Anything inside `<!--        -->` is percieved as comment by HTML document.
