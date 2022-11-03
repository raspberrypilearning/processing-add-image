### Een afbeelding uploaden

Als je jouw eigen afbeelding wilt gebruiken, kun je dat doen door op de knop 'Afbeeldingen bekijken en toevoegen' te klikken.

![Een plusteken, een uploadsymbool en een afbeeldingssymbool. Het afbeeldingssymbool is gemarkeerd.](images/trinket_image.png)

Kies vervolgens 'Image Library' en volg de instructies op het scherm om een afbeelding te uploaden naar je Trinket-afbeeldingenbibliotheek.

![Een knop met een plusje en de woorden 'Image Library' erop.](images/trinket_image_library.png)

**Tip:** Noteer de bestandsnaam van de afbeelding die je hebt geüpload, omdat je die in de code gaat gebruiken.

### Afbeeldingscode toevoegen

Go to the setup() function and add code, create a new global variable and load the image in:

--- code ---
---
language: python filename: main.py - setup()

---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

Voeg de functie `image()` toe op de plek in de code waar je jouw afbeelding wilt tekenen.

De functie `image()` is als volgt ingedeeld:

`image(bestandsnaam afbeelding, x-coördinaat, y-coördinaat, afbeeldingsbreedte, afbeeldingshoogte)`

De coördinaten positioneren de linkerbovenhoek van de afbeelding.

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![Het codeveld en het uitvoerveld met getoonde afbeelding van een robot.](images/inserted-robot.png)
