<sub>Think you might be in the wrong place? [Go home!](README.md)</sub>
### What is the purpose of CSS?
The purpose of CSS _(Cascading Style Sheets)_ is to control the presentation and formatting of web documents written in HTML and XML.
### What are the three ways to insert CSS into your project?
* ### Inline CSS: 
<p> Adding CSS directly to individual HTML elements using the style attribute. Suitable for specific, one-off style changes.</p>

* ### Internal or Embedded CSS: 
Placing CSS code within the <style> element in the HTML document's <head>. Useful for applying styles to a single web page.

* ### External CSS:

 Creating a separate CSS file with a .css extension and linking it to HTML documents using the <link> element. This is the recommended method for larger projects, promoting code organization and reusability.

### Write an example of a CSS rule that would give all <p> elements red text.
p{
    color: red;
}