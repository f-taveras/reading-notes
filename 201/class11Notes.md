<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### Explain how the ability to use video and audio on the web has evolved since the early 2000s.

 Web multimedia has come a long way since the early 2000s. HTML5 introduced native support for video and audio, replacing the need for plug-ins like Flash. This standardization made multimedia content accessible and seamless.

 The shift to HTML5 has further improved the performance and quality of multimedia content. It introduced support for various codecs and streaming protocols, allowing for higher-quality video and audio delivery while optimizing performance. This evolution has empowered web developers to create multimedia-rich websites that cater to a broader audience.

### Describe the use of the src and controls attributes in the \<video> element.

In the __\<video>__ element, the src attribute specifies the video source, and controls adds playback controls. For example:

 <video src="myvideo.mp4" controls></video>.

### Why is it important to have fallback content inside the __\<video>__ element?
 Fallback content in __\<video>__ provides an alternative experience for users with unsupported browsers. It enhances accessibility and ensures everyone can access the content.

### Write a very short story where __\<audio>__ and __\<video>__ are characters.

In the digital realm, \<audio> and \<video> were inseparable companions, creating captivating web experiences. \<audio> played music and narrated stories, while \<video> brought tales to life. Together, they enchanted the web, one click at a time.

### How does Grid layout differ from Flex?

Grid Layout and Flexbox are CSS layout models, each serving distinct purposes.

* __Grid Layout:__ It's for two-dimensional layouts with rows and columns. Perfect for grid structures, like spreadsheets or card-based designs.

* __Flexbox:__ Designed for one-dimensional layouts, often used for arranging items in a row or column. Great for responsive design and aligning content along a single axis.

### Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.
 
* __Grid Container:__ An HTML element designated as the parent of a grid layout, created with display: grid;.

* __Grid Item:__ Immediate child elements of a grid container, placed within grid cells for complex layouts.

* __Grid Line:__ The lines that form grid rows and columns, numbered or named, used for positioning and sizing grid items.



### Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

Responsive images benefit performance, user experience, and SEO. They load smaller images for smaller screens, reducing data transfer.

### Define the following __\<img>__ attributes "srcset" and "sizes". Write an example of how they are used.

* __srcset__ specifies image sources with different sizes and lets the browser choose the right one.
* __sizes__ defines image display sizes relative to viewport width.

Example:

```
<img src="image-small.jpg" srcset="image-medium.jpg 800w, image-large.jpg 1200w" sizes="(max-width: 600px) 100vw, 50vw" alt="Responsive Image"/>
```

### How is "srcset" more helpful for responsive images than CSS or JavaScript?

* Simplifies responsive images.
* Better file selection for performance.
* Reduces data transfer and improves page load times.
* In short, responsive images improve performance, user experience, and SEO.  
* _srcset_ and _sizes_ simplify implementation, letting the browser handle image selection for better performance.

<sub>Information gathered using ChatGPT</sub>