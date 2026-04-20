# mkdocs 導入手順

## Pythonダウンロード

**直接ダウンロード**

https://www.python.org/ftp/python/3.13.13/python-3.13.13-amd64.exe

**↑のリンク元のページ**

https://www.python.org/downloads/windows/

## インストーラーexeファイル実行

- 「?Add Python to PATH 」にチェック
- 「Install Now」でOK

## インストール後、コマンドプロンプトから以下を実行

```
python --version
```

※1 エラーが出てたらＰＣ再起動

※2 再起動でもエラーが表示されたら、システム環境変数のPathを確認

## pipのバージョン確認

```
py -m pip --version
py -m pip install --upgrade pip
```

## mkdocs インストール

```
py -m pip install mkdocs-material
```

## プロジェクト作成

```
cd <任意の場所>
mkdocs new <プロジェクト名>
cd <プロジェクト名>
```

以下のディレクトリが生成される

my-project/

├─ docs/

│   └─ index.md   ← メインファイル

└─ mkdocs.yml   ← ルート設定

## <プロジェクト名>ディレクトリ内で以下実行

```
mkdocs serve
```

ブラウザで動作確認

http://127.0.0.1:8000/

## 編集

docs/ 内でページの数だけファイルを増やす

mkdocs.yml でページへのリンクを設定
