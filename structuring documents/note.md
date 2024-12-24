# Basic Sections of a Document
<dl>

<dt> header: </dt>
<dd> 
Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one page of a website to another. 
</dd>

<dt> navigation bar: </dt>
<dd> 
Links to the site's main sections; usually represented by menu buttons, links, or tabs. Like the header, this content usually remains consistent from one webpage to another — having inconsistent navigation on your website will just lead to confused, frustrated users. Many web designers consider the navigation bar to be part of the header rather than an individual component, but that's not a requirement; in fact, some also argue that having the two separate is better for accessibility, as screen readers can read the two features better if they are separate. 
</dd>

<dt> main content: </dt>
<dd> 
A big area in the center that contains most of the unique content of a given webpage. This part of website varies from page to page 
</dd>

<dt> side bar: </dt>
<dd>
 Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system. 
 </dd>

<dt> footer: </dt>
<dd>
A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself. The footer is also sometimes used for SEO purposes, by providing links for quick access to popular content.
</dd>

</dl>

# HTML for structuring content
- In your HTML code, you can mark up sections of content based on their functionality — you can use elements that represent the sections of content described above unambiguously, and assistive technologies like screen readers can recognize those elements and help with tasks like "find the main navigation", or "find the main content." 

- To implement such semantic mark up, HTML provides dedicated tags that you can use to represent such sections, for example:

- header: `<header>`
- navigation bar: `<nav>`
- main content: `<main>` with various sub-sections represented by `<article>`, `<section>` and `<div>` elements
- sidebar: `<aside>` often placed inside main
- footer: `<footer>`

# HTML layout elements in more detail
- `<main>` is for content unique to this page. Use `<main>` only once per page, and put it directly inside `<body>`. Ideally this shouldn't be nested within other elements.

- `<article>` encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).

- `<section>` is similar to `<article>`, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's considered best practice to begin each section with a heading; also note that you can break `<article>`s up into different `<section>`s, or `<section>`s up into different `<article>`s, depending on the context.

- `<aside>` contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).

- `<header>` represents a group of introductory content. If it is a child of `<body>` it defines the global header of a webpage, but if it's a child of an `<article>` or `<section>` it defines a specific header for that section (try not to confuse this with titles and headings).

- `<nav>` contains the main navigation functionality for the page. Secondary links, etc., would not go in the navigation.

- `<footer>` represents a group of end content for a page.

# Non Semantic Wrappers
- HTML provides the `<div>` and `<span>` elements. You should use these preferably with a suitable class attribute, to provide some kind of label for them so they can be easily targeted.

- `<span>` is an <u>inline</u> non-semantic element, which you should only use if you can't think of a better semantic text element to wrap your content, or don't want to add any specific meaning. 

- `<div>` is a <u>block</u> level non-semantic element, which you should only use if you can't think of a better semantic block element to use, or don't want to add any specific meaning.

# The line break and Horizontal Rule
## `<br>`: Line break element
- As HTML ignores the white-spaces, `<br>` is one of the only way to force a rigid structure in a situation where you want a series of fixed short lines.

- This tag creates a line break in a paragraph. 

## `<hr>`: Horizontal Rule
- The tag `<hr>` creates a horizontal rule that denotes a thematic change in the text such as change in topic or scenes in scripts.

# Planning a Simple Website
- You'll have a few elements common to most (if not all) pages — such as the navigation menu, and the footer content. If your site is for a business, for example, it's a good idea to have your contact information available in the footer on each page. Note down what you want to have common to every page.

- Next, draw a rough sketch of what you might want the structure of each page to look like (it might look like our simple website above). Note what each block is going to be.

- Now, brainstorm all the other (not common to every page) content you want to have on your website — write a big list down.

- Next, try to sort all these content items into groups, to give you an idea of what parts might live together on different pages. This is very similar to a technique called Card sorting.

- Now try to sketch a rough sitemap — have a bubble for each page on your site, and draw lines to show the typical workflow between pages. The homepage will probably be in the center, and link to most if not all of the others; most of the pages in a small site should be available from the main navigation, although there are exceptions. You might also want to include notes about how things might be presented.