### Llwytho delwedd i fyny

Os ydych chi am ddefnyddio eich delwedd eich hun, fe allwch chi wneud hynny drwy ddewis y botwm ‘View and add images’.

![Symbol plws, symbol llwytho i fyny, a symbol delwedd. Mae'r symbol delwedd wedi'i amlygu.](images/trinket_image.png)

Yna dewiswch 'Image Library' a dilyn y cyfarwyddiadau ar y sgrin i lwytho delwedd i fyny i'ch llyfrgell delweddau Trinket.

![Botwm gydag arwydd plws a'r geiriau 'Image Library' arno.](images/trinket_image_library.png)

**Cyngor:** Gwnewch nodyn o enw ffeil y ddelwedd rydych chi wedi'i llwytho i fyny, oherwydd byddwch chi'n ei ddefnyddio yn y cod.

### Ychwanegu cod delwedd

Go to the setup() function and add code, create a new global variable and load the image in:

--- code ---
---
language: python filename: main.py - setup()

---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

Ychwanegwch y swyddogaeth `image()` at y man yn y cod lle rydych chi am lunio eich delwedd.

Mae'r swyddogaeth `image()` wedi'i gosod fel:

`image(image filename, x-coordinate, y-coordinate, width, height)`

Mae'r cyfesurynnau'n lleoli cornel chwith uchaf y ddelwedd.

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![Yr ardal cod a'r ardal allbwn gyda delwedd o robot wedi'i dangos.](images/inserted-robot.png)
