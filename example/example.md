# A Markdown file with links to images

This is a sample file written in Markdown that links to images.

## Basic image display

For basic images, use Markdown itself: `![alt text](image-url)`. The `alt text` appears if the image can't be found, and is read aloud by screen readers. The `image-url` is the path to the image. If the image is in the same folder as the Markdown file, you only need the name of the image file.

![A smiling face](Face-smile.png)

## Image display with HTML and CSS

If you want to do fancy stuff — resizing, floating an image alongside text, centering — then you have to switch to HTML/CSS code snippets. One caveat is that GitHub sanitizes HTML for security reasons, allowing only a limited set of CSS properties. Anything outside that set is silently discarded, so you won't get the full benefit of CSS. For most things, though, what GitHub allows is sufficient.

Be aware that editors like Visual Studio Code, which have Markdown preview tools, may support a wider range of CSS than GitHub does. Always double-check your document on GitHub.

The examples below are enough to get you started. Experiment to find other options.

You will need to view the raw Markdown to see the HTML code.

### Centering images

To center an image, wrap it in a paragraph with the `align` attribute:

<p align="center">
  <img src="Face-smile.png" alt="A centered smiley face">
</p>

### Resizing images

You can size an image as a percentage of its container. Here, the container is the width of the page.

<img src="Face-smile.png" style="width:50%;" alt="A large smiley face">

### Float an image to the left or right

To wrap text around an image — text on the left, image on the right — you can't use CSS's `float:right`, as GitHub strips it. Use the HTML attribute `align="right"` instead:

<img src="Face-smile.png" align="right" style="margin-left: 1em; margin-bottom: 1em;" alt="A smiley face on the right">

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum rhoncus ultrices nunc, nec fermentum massa porttitor sit amet. Etiam vehicula, neque sed auctor euismod, tellus est ullamcorper enim, ac elementum nibh libero in odio. Ut ultrices urna at placerat interdum. Sed at tempus lectus, quis semper enim. Proin eu ante nunc. Curabitur mattis dui pharetra, posuere magna vel, venenatis leo. Aliquam erat volutpat. Aliquam sed lectus ac turpis aliquet ultrices sit amet vitae turpis. Vivamus eu congue nunc. Maecenas eleifend blandit nisl, non egestas felis lacinia sit amet. Nulla congue arcu eget consectetur malesuada.

---

The horizontal rule above clears the float, so the next section starts below the image rather than continuing to wrap around it.

### Caption an image

In many cases you will want to give an image a caption. You can use HTML's `figure` element:

<figure align="center">
  <img src="Face-smile.png" alt="A smiling face">
  <figcaption>Figure 1: A smiling face.</figcaption>
</figure>

In general, captioned figures should be centered.

### Add images within text

By default, the `img` element is an inline element, which means it can sit inside a paragraph and flow with the surrounding text. Setting `height: 1em` in the code below scales the image to match the font size of the text around it.

When you see a smile <img src="Face-smile.png" style="height: 1em" alt="A small smiley face"> it makes you happy!