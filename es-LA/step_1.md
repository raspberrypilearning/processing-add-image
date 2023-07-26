### Sube una imagen

Si quieres usar tu propia imagen, puedes hacerlo eligiendo el botón 'View and add images' (Ver y agregar imágenes).

![Un signo de suma, un símbolo de subir y un símbolo de imagen. El símbolo de la imagen está resaltado.](images/trinket_image.png)

Luego elige 'Image Library' (Biblioteca de imágenes) y sigue las instrucciones en pantalla para cargar una imagen a tu biblioteca de imágenes de Trinket.

![Un botón con un signo de suma y las palabras "Image Library".](images/trinket_image_library.png)

**Sugerencia:** Toma nota del nombre de archivo de la imagen que subiste, ya que la usarás en el código.

### Agrega código de imagen

Ve a la función setup() y agrega código, crea una nueva variable global y carga la imagen en:

--- code ---
---
language: python filename: main.py - setup()

---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

Agrega la función `imagen()` al lugar del código donde quieras dibujar tu imagen.

La función `imagen()` se dispone así:

`imagen(nombre del archivo de imagen, coordinada-x, coordinada-y, ancho, alto)`

Las coordenadas posicionan la parte superior izquierda de la imagen.

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![Se muestra el área de código y el área de salida con la imagen del robot.](images/inserted-robot.png)
