### Télécharger une image

Si tu souhaites utiliser ta propre image, tu peux le faire en choisissant le bouton "View and add images".

![Un plus, un symbole de téléchargement et un symbole d'image. Le symbole de l'image est mis en surbrillance.](images/trinket_image.png)

Choisis ensuite Image Library et suis les instructions à l'écran pour télécharger une image dans ta bibliothèque d'images Trinket.

![Un bouton avec un plus et les mots "Image Library" dessus.](images/trinket_image_library.png)

**Astuce :** Note le nom de fichier de l'image que tu as téléchargée car tu l'utiliseras dans le code.

### Ajouter un code d'image

Accéde à la fonction setup() et ajoute du code, crée une nouvelle variable globale et charge l'image dans :

--- code ---
---
language: python 
filename: main.py - setup()

---

def setup(): 
  global robot 
  robot = load_image('robot.png')

--- /code ---

Ajoute la fonction `image()` à l'endroit du code où tu veux dessiner ton image.

La fonction `image()` se présente comme suit :

`image(nom du fichier image, coordonnée x, coordonnée y, largeur, hauteur)`

Les coordonnées positionnent le coin supérieur gauche de l'image.

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![La zone de code et la zone de sortie avec l'image du robot affichée.](images/inserted-robot.png)

