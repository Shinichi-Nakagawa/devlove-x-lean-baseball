# DevLOVE X 2019.06.23

[DevLOVE X](https://devlove.wixsite.com/devlovex)登壇資料.

Jupyter notebookとして動きます.

## 使い方

### Github・nbviewer上でそのまま読む

この場合は特にPythonライブラリ・環境は必要ありません.

そのままURLをたどって読んでください.

### 手元で動かす

この場合はPython環境が必要です.

## 手元で動かす場合の設定

Python3を使える環境を作って必要なライブラリをpip installしてください.

仮想環境(venv)利用を推奨ですが, [Anaaconda](https://www.python.jp/install/anaconda/index.html)等を使ってもかまいません.

※ここではvenvを前提として手順を記載

### Python 3のインストール

最新版を使いましょう.執筆時点(2019.06.23)では3.7が最新となります.

[Pythonをインストール(by python.jp)](https://www.python.jp/install/windows/install_py3.html)

### 仮想環境を作る

任意のディレクトリの下にvenvで仮想環境を構築.

仮想環境の名前は「devlove」とします.

※devlove以外の名前でもOKです(変更の場合は以降を読み替えて)

```bash
$ # この例では ~/python_venv を仮想環境のディレクトリとします
$ python3 -m venv ~/python_venv/devlove
$ source ~/python_venv/devlove/bin/activate
```

念の為whichコマンドでpython/pipが然るべきところに通ってる所を確認

```bash
(devlove) $ which python
(devlove) $ which pip
```

### ライブラリをインストール

requirements.txtに必要なライブラリがあるのでそれを使ってインストールします.

```bash
(devlove) $ pip install -r requirements.txt
```

ちなみに, 同包しているrequirements.inは[pip-tools](https://pypi.org/project/pip-tools/)用の設定です.

### Jupyter notebookとして起動

```bash
(devlove) $ jupyter notebook
```
