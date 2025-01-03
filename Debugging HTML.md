# Debugging HTML
HTML is not compiled into a different form before the browser parses it and shows the result (it is interpreted, not compiled). And HTML's element syntax is arguably a lot easier to understand than a "real programming language" like Rust, JavaScript, or Python. The way that browsers parse HTML is a lot more permissive than how programming languages are run, which is both a good and a bad thing.

# Permissive Code
 Generally when you do something wrong in code, there are two main types of error that you'll come across:
 - Syntax errors: These are spelling or punctuation errors in your code that actually cause the program not to run. These are usually easy to fix as long as you are familiar with the language's syntax and know what the error messages mean.
 - Logic errors: These are errors where the syntax is actually correct, but the code is not what you intended it to be, meaning that the program runs incorrectly. These are often harder to fix than syntax errors, as there isn't an error message to direct you to the source of the error.

 HTML itself doesn't suffer from syntax errors because browsers parse it permissively, meaning that the page still displays even if there are syntax errors. Browsers have built-in rules to state how to interpret incorrectly written markup, so you'll get something running, even if it is not what you expected. This, of course, can still be a problem!

The best strategy is to start by running your HTML page through the <a href="https://validator.w3.org/"> Markup Validation Service </a> — created and maintained by the W3C, the organization that looks after the specifications that define HTML, CSS, and other web technologies. This webpage takes an HTML document as an input, goes through it, and gives you a report to tell you what is wrong with your HTML.