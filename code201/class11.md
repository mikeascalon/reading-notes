# Reading Notes

## Audio, Video, Images

1.Explain how the ability to use video and audio on the web has evolved since the early 2000s.

* the ability to use video and audio on the web has evolved from reliance on plugins like Flash to the widespread use of native HTML5 elements and modern web technologies

2.Describe the use of the src and controls attributes in the `<video>` element.

* src - attribute contains a path to the video you want to embed

* controls -attribute is a boolean attribute that, when present, adds a set of playback controls to the video player

3.Why is it important to have fallback content inside the `<video>` element?

* this will be displayed if the browser accessing the page doesn't support the `<video>` element, allowing us to provide a fallback for older browsers.

4.Write a very short story where `<audio>` and `<video>` are characters.

* `<audio>` and `<video>` were like two heroic soldiers on a critical mission. `<audio>`, with its powerful voice, carried the stories and messages of the kingdom's people, inspiring courage in the face of adversity.`<video>`, a visual storyteller, painted vivid pictures of the challenges they faced.

## A Complete Guide To Grid

1.How does Grid layout differ from Flex?

* Grid layout is best for two-dimensional layouts, where you need to manage both rows and columns, and it's suitable for the overall structure of a page. Flexbox, on the other hand, is ideal for one-dimensional layouts, useful for aligning and distributing items along a single axis within specific sections or components of a page.

2.Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

* Grid container is an HTML element that is designated as a grid by applying the display: grid; property in its CSS.

* Grid items are the immediate children of a grid container. They are the elements that are placed within the grid layout.

* Grid lines are the horizontal and vertical lines that form the grid structure. They separate rows and columns within the grid.

## Responsive Images

1.Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

* Responsive images ensure that the content is accessible and readable on a wide range of devices, from large desktop monitors to small mobile screens.

2.Define the following `<img>` attributes srcset and sizes. Write an example of how they are used.

* The srcset attribute specifies a list of image files, along with their respective descriptors for the image's pixel density (or resolution).

* The sizes attribute defines the sizes of the image in layout units (typically, in CSS units like vw for viewport width) that the image will occupy in the layout.

* The sizes attribute specifies how the image will be displayed in the layout.

* The srcset attribute offers three alternative image options with descriptors for their widths:

3.How is srcset more helpful for responsive images than CSS or JavaScript?

It simplifies the process, enhances performance, and ensures that users receive the best image quality for their specific viewing context, making it a preferred choice for responsive web design.

### Resources

[Video and audio content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

[A Complete Guide to CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

[Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
