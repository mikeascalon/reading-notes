# Reading Notes #5

## HTML Media

1.What is a real world use case for the alt attribute being used in a website?

Search engines also read image filenames and count them towards SEO. Therefore, you should give your image a descriptive filename

2.How can you improve accessibility of images in an HTML document?

* Use the alt Attribute

* Use Descriptive Filenames

* Provide Longer Descriptions

* Decorative Images

3.Provide an example of when the figure element would be useful in an HTML document.

```javascript
<figure>
  <img
    src="dinosaur.png"
    alt="The Mozilla Tyrannosaurus"
    aria-describedby="dinodescr" />
  <figcaption id="dinodescr">
    A red Tyrannosaurus Rex: A two legged dinosaur standing upright like a
    human, with small arms, and a large head with lots of sharp teeth.
  </figcaption>
</figure>

```

4.Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

* GIF is like a flipbook of pictures that play one after the other.
SVG is a drawing or painting that's made of lines and shapes.

5.What image type would you use to display a screenshot on your website and why?

* PNG  images use lossless compression, meaning they maintain the image quality without losing detail or introducing artifacts.

## Learn CSS

1.Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

* The Background color is like the color of your car and the foreground is the color of the decal of your car.

2.Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

* I would ask first what kind of theme he has in mind. once I get a idea of the color scheme . I’ll will apply the colors on the background , header , and font color.

3.What should you consider when choosing fonts for an HTML document?

* Consider the web safe fonts.

4.What do font-size, font-weight, and font-style do to HTML text elements?

* font-size affects the size of the font.

* font-weight It sets how bold is the text.

* font-style- affects the font if it's bold or italic.

5 Describe two ways you could add spacing around the characters displayed in an h1 element.

* you can put some padding and margin around h1

### Resources

[HTML Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

[Fundamental text and font styling](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)