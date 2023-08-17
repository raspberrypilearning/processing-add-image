### Fazer upload de uma imagem

Se você quiser usar sua própria imagem, pode fazer isso clicando no botão "View and add images".

![Um símbolo de adição, um símbolo de upload e um símbolo de imagem. O símbolo de imagem está realçado.](images/trinket_image.png)

Em seguida, clique em "Image Library" e siga as instruções na tela para fazer upload de uma imagem para sua biblioteca de imagens Trinket.

![Um botão com um sinal de adição e as palavras "Image Library" nele.](images/trinket_image_library.png)

**Dica:** Anote o nome do arquivo da imagem que você fez o upload, pois você o usará no código.

### Adicionar código da imagem

Vá para a função setup() e adicione o código, crie uma nova variável global e carregue a imagem em:

--- code ---
---
language: python
filename: main.py - setup()

---

def setup():
  global robo
  robo = load_image('robot.png')

--- /code ---

Adicione a função `image()` no código onde você deseja desenhar sua imagem.

A função `image()` é apresentada:

`image(nome do arquivo de imagem, coordenada x, coordenada y, largura, altura)`

As coordenadas posicionam o canto superior esquerdo da imagem.

--- code ---
---
language: python

---

  image(robo, 50, 50, 300, 300)

--- /code ---

![A área de código e a área de saída mostrando a imagem do robô.](images/inserted-robot.png)
