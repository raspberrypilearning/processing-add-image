### Upload an image

If you want to use your own picture, you can do that by choosing the ‘View and add images’ button.

![A plus, an upload symbol, and an image symbol. The image symbol is highlighted.](images/trinket_image.png)

Then choose ‘Image Library’ and follow the on-screen instructions to upload an image to your Trinket image library.

![A button with a plus and the words 'Image Library' on it.](images/trinket_image_library.png)

**Tip:** Make a note of the filename for the image you’ve uploaded as you will use it in the code.

### Add image code

Go to the setup() function and add code create a new global variable and load the image in:

--- code ---
---
language: python filename: main.py - setup()

---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

Add the `image()` function to the place in the code where you want to draw your image.

The `image()` function is laid out:

`image(image filename, x-coordinate, y-coordinate, width, height)`

The coordinates position the top-left of the image.

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![The code area and output area with robot image shown.](images/inserted-robot.png)
