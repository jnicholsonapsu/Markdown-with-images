# A Markdown file with links to images

This is a sample file written in Markdown that links to images. 

For basic images use markdown itself, `![alt text](image url)`. The `alt text` appears if the image can't be found. The `image url` is the path to the image. If the image is in the same folder as the markdown file, you only need the name of the image file.

![A smiling face](Face-smile.png)

If you want to do fancy stuff, e.g., resizing, making the image float around text, centering, then you have to switch to using HTML code snippets with inline CSS.

For example, if you wanted to center an image, you can do this:

<img src="Face-smile.png" style="display:block;margin:auto;" alt="A centered smiley face">

If you want to resize the image, you can do  resize the image to a percentage of its container (the container here is the whole page.)

<img src="Face-smile.png" style="width:50%;" alt="A big smiley face">

If you want an image to float around text, e.g., text on the left and image on the right.  You can't use CSS's `float:right` as GitHub strips that, but you can use the HTTML attribute `align="right"`. For example, 

<img src="Face-smile.png" align="right" style="margin-left: 1em; margin-bottom: 1em;" alt="A centered smiley face">

 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum rhoncus ultrices nunc, nec fermentum massa porttitor sit amet. Etiam vehicula, neque sed auctor euismod, tellus est ullamcorper enim, ac elementum nibh libero in odio. Ut ultrices urna at placerat interdum. Sed at tempus lectus, quis semper enim. Proin eu ante nunc. Curabitur mattis dui pharetra, posuere magna vel, venenatis leo. Aliquam erat volutpat. Aliquam sed lectus ac turpis aliquet ultrices sit amet vitae turpis. Vivamus eu congue nunc. Maecenas eleifend blandit nisl, non egestas felis lacinia sit amet. Nulla congue arcu eget consectetur malesuada.
