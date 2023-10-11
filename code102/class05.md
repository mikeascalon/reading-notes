# Reading Notes 05

## Read: 05 - Design web pages with CSS

1.What is the purpose of CSS?

Color to text , styles our pages

2.What are the three ways to insert CSS into your project?

 a.External CSS

- you can change the look of an entire website by changing just one file!
Each HTML page must include a reference to the external style sheet file inside the `<link>` element, inside the head section.

 b.Internal CSS

- An internal style sheet may be used if one single HTML page has a unique style.
The internal style is defined inside the `<style> element`, inside the head section.

 c.Inline CSS

- An inline style may be used to apply a unique style for a single element.
To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

3.Write an example of a CSS rule that would give all `<p>` elements red text.

`<style>`

`p {`
  
  `color: red;`

`}`

`</style>`
