# A Markdown file with links to images

This is a sample file written in Markdown that links to images. 

For basic images use markdown itself, `![alt text](image url)`. The `alt text` appears if the image can't be found. The `image url` is the path to the image. If the image is in the same folder as the markdown file, you only need the name of the image file.

![A smiling face](Face-smile.png)

If you want to do fancy stuff, e.g., resizing, making the image float around text, centering, then you have to switch to using HTML code snippets with inline CSS.

For example, if you wanted to center an image, you can do this:

<img src="Face-smile.png" style="display:block;margin:auto;" alt="A centered smiley face">

If you want to resize the image, you can do  resize the image to a percentage of the page

<img src="Face-smile.png" style="width:50%;" alt="A centered smiley face">

