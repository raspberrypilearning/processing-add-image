### 画像をアップロードする

自分の画像を使いたい場合は「View and add images」ボタンを選択します。

![プラス記号、アップロード記号、および画像記号。 画像記号が強調表示されている。](images/trinket_image.png)

続いて「Image Library」を選択し、画面の指示に従って画像をTrinket Image Libraryにアップロードします。

![プラス記号と「Image Library」という言葉が書かれたボタン。](images/trinket_image_library.png)

**ヒント：**コード中で使うので、アップロードした画像のファイル名をメモしておきます。

### 画像コードを追加する

setup()関数へ移動して、新しいグローバル変数を作成し、その変数に画像を読み込むコードを追加します。

--- code ---
---
language: python filename: main.py - setup()

---

def setup(): global robot robot = load_image('robot.png')

--- /code ---

画像を描画したいコード中の場所に`image()`関数を追加します。

`image()`関数の構成は以下のとおりです。

`image(画像ファイル名, x座標, y座標, 画像の幅, 画像の高さ)`

座標は画像の左上に配置されます。

--- code ---
---
language: python

---

  image(robot, 50, 50, 300, 300)

--- /code ---

![ロボット画像が表示されたコード領域と出力領域。](images/inserted-robot.png)
