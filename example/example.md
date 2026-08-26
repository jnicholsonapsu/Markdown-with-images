# A Markdown file with links to images

This is a sample file written in Markdown that links to images. 

## Basic image display

For basic images use markdown itself, `![alt text](image url)`. The `alt text` appears if the image can't be found. The `image url` is the path to the image. If the image is in the same folder as the markdown file, you only need the name of the image file.  

![A smiling face](Face-smile.png)

## Image display with HTML and CSS

If you want to do fancy stuff, e.g., resizing, making the image float around text, centering, then you have to switch to using HTML/CSS code snippets. One caveat to this is that GitHub strips some CSS for security reasons. Meaning you won't get the full benefit of CSS. But for most things, the CSS that GitHub allows is sufficient. Be aware that editors like Visual Studio Code that have Markdown preview tools may support a wider range of CSS that GitHub. Always double-check your document on GitHub.

The examples below are enough to get you started.  Experiment to find other options.

You will need to view the raw Markdown to see the HTML code.

### Centering images

If you want to center an image, you can do this:

<img src="Face-smile.png" style="display:block;margin:auto;" alt="A centered smiley face">

### Resizing images

If you want to resize the image, you can resize the image to a percentage of it's container (here, the container is the whole page.)

<img src="Face-smile.png" style="width:50%;" alt="A big smiley face">

### Float an image to the left or right

If you want an image to float around text, e.g., text on the left and image on the right.  You can't use CSS's `float:right` as GitHub strips that, but you can use the HTTML attribute `align="right"`. For example, 

<img src="Face-smile.png" align="right" style="margin-left: 1em; margin-bottom: 1em;" alt="A smiley face on the right">

 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum rhoncus ultrices nunc, nec fermentum massa porttitor sit amet. Etiam vehicula, neque sed auctor euismod, tellus est ullamcorper enim, ac elementum nibh libero in odio. Ut ultrices urna at placerat interdum. Sed at tempus lectus, quis semper enim. Proin eu ante nunc. Curabitur mattis dui pharetra, posuere magna vel, venenatis leo. Aliquam erat volutpat. Aliquam sed lectus ac turpis aliquet ultrices sit amet vitae turpis. Vivamus eu congue nunc. Maecenas eleifend blandit nisl, non egestas felis lacinia sit amet. Nulla congue arcu eget consectetur malesuada.

### Caption an image

In many cases, you will need to give an image a caption.  For that you can use HTML's `figure` element. For example:

<figure>
  <img src="Face-smile.png" alt="A smiling face">
  <figcaption>Figure 1: A smiling face.</figcaption>
</figure>

### Add images in text

By default, the `IMG` element is an inline element. This means it can act like text in things like paragraphs.  The `1em` in the code make the `height` of the image the same as the max height of the text.

When you see a smile <img src="Face-smile.png" style="height: 1em" alt="A big smiley face"> it makes you happy!

