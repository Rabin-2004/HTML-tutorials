# Hyperlink 
-  Hyperlinks allow us to link documents to other documents or resources, link to specific parts of documents, or make apps available at a web address. Almost any web content can be converted to a link so that when clicked or otherwise activated the web browser goes to another web address.

# URL and Paths
- A URL, or Uniform Resource Locator is a string of text that defines where something is located on the Web. For example, Google's homepage is located at https://www.google.com/.
- URLs use paths to find files. Paths specify where the file you're interested in is located in the filesystem.

# Absolute and Relative URLs
- Absolute URL points to a location defined by its absolute location on the web, including protocol and domain name. For example, if an index.html page is uploaded to a directory called projects that sits inside the root of a web server, and the website's domain is https://www.example.com, the page would be available at https://www.example.com/projects/index.html.
- Relative URL points to a location that is relative to the file you are linking from. For eg: if you have a file index.html inside a folder src and you want to link to a file index2.html inside a folder components inside the same root directory then the relative url would be './components/index2.html'

# Link best practices
- ## Use clear link wording
- Example: 
` <p> <a href= 'https://www.google.com'> Go to Google </a> </p>` is a good link text.
`<p> <a href= 'https://www.google.com'> Click Here </a> to go to Google</p>` is a bad link text.
- Use consice wordings and text to make links more accesible for screen readers.

- ## Other tips:
- Don't repeat the URL as part of the link text — a screen reader reads them out letter by letter.
- Don't say "link" or "links to" in the link text. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
- Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
- Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here"