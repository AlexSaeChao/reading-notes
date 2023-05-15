# Audio, Video, Images

Audio videos and images are a large part in how we share and consume information. There are many ways to display them effectively with layouts and size of the material.

## Video and Audio Content

Explain how the ability to use video and audio on the web has evolved since the early 2000s.

The old stuff like flash and silverlight has security issues and was resource intensive. they now have the widespread adoption of h.264 video codec and AAC audio codecs. flash also had to be downloaded separately.

Describe the use of the src and controls attributes in the `<video>` element.

the src is attributes has the path to the video you want to embed just like in an img element. The control attribute includes the browser's own control interface, otherwise you would have to make your own with the appropriate JavaScript API.

Why is it important to have fallback content inside the `<video>` element?

IF the browser does not support HTML5 then a fallback content should have a message stating so and a link to the video.

Write a very short story where `<audio>` and `<video>` are characters.

The days when it first started, was a bit odd. Video and Audio never understood what security actually meant. On older machines to this they would siphon resources and cause crashes. because of this both of them got a few unkind words thrown back at them. Video was the older, audio was its younger fraternal twin. They were quite gullible from others who wanted to take advantage of what they were trying to accomplish. They really just wanted to share information in forms of words and sounds, while the older sibling shared just same just with pictures frame by frame. Eventually they found people that wanted to help them with their quest. From past experiences and the support of others, they both learned they didn't have to trust everyone to spread the word of the world. with their framework of help they could now execute their mission without others impeding them. Having worked efficiently on their business they could help others now without having to use so much from the ones who listen or view.

## A Complete Guide To Grid

How does Grid layout differ from Flex?

Grids are a 2-D system that allows layouts with rows and columns, and flexbox works on a one-dimensional system, a single row or column that is more focused on the arrangement of elements, Flew box has done a few things well like making flexible and scalable layout designs that shrink with the view window while the grid layout can do something similar with help from CSS and JS.  

Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

* Grid container: an element that becomes a grid context for its direct child elements using the `display; grid` in the css property. The children of this container are referred to as grid items.
* Grid items: immediate children of a grid container, they can live on multi rows or columns merged, occupying specific areas of the grid layout.
* Grid line: make up the grid structure. They move from top to bottom left to right starting at an index of 1. Gridlines can be referred by using positive numbers or  negative numbers which start counting from the end of the grid.

## Responsive Images

Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

They help with loading times, accessibility, make elements act as intended across most/all devices. SEO considers load times as well.

Define the following `<img>` attributes srcset and sizes. Write an example of how they are used.

* src is the images source, some browsers don't support srcset.
* srcset has a list of alternative sizes provided; small, med, lrg.
* sizes are based on vw or viewport width.

On a mobile device, smaller images help the loading and responsiveness, using less resources of the device.

``` html
<img src="image.jpg" 
     srcset="image-small.jpg 320w,
             image-medium.jpg 768w,
             image-large.jpg 1200w"
     sizes="(max-width: 768px) 100vw,
            (max-width: 1200px) 50vw,
            33vw"
```

How is srcset more helpful for responsive images than CSS or JavaScript?

Together you can specific what device your using and choose which combination of srcset and sizes to make the UX much more appealing on the certain device. It allows the browser to choose the best one without additional code.

### Things I want to know more about

Is there a way to combine graphic design elements in the production of a webpage more efficiently without so much code.