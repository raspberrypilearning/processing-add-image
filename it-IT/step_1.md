### Carica un'immagine

Se desideri utilizzare una tua immagine, puoi farlo cliccando il pulsante "Visualizza e aggiungi immagini".

![Un segno più, un simbolo di caricamento e un simbolo di immagine. Il simbolo dell'immagine è evidenziato.](images/trinket_image.png)

Quindi scegli "Image Library" e segui le istruzioni visualizzate sullo schermo per caricare un'immagine nella tua libreria di immagini Trinket.

![Un pulsante con un segno più e la scritta "Image Library".](images/trinket_image_library.png)

**Suggerimento:** Prendi nota del nome del file dell'immagine che hai caricato poiché lo utilizzerai nel codice.

### Aggiungi il codice per l'immagine

Vai alla funzione setup() e aggiungi il codice, crea una nuova variabile globale e carica l'immagine in:

--- code ---
---
language: python filename: main.py - setup()
---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

Usa la funzione `image()` nel punto del codice in cui desideri disegnare la tua immagine.

La funzione `image()` è così strutturata:

`image(nome immagine, coordinata x, coordinata y, larghezza, altezza)`

Le coordinate indicano l'angolo in alto a sinistra dell'immagine.

--- code ---
---
language: python
---

  image(robot, 50, 50, 300, 300)

--- /code ---

![L'area del codice e l'area di output con l'immagine del robot mostrata.](images/inserted-robot.png)
