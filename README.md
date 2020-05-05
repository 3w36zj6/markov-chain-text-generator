# Text Generator
マルコフ連鎖を使った文章自動生成プログラム

## 使い方
文章の自動生成の方法

### 事前準備
`text.txt`に元になる文章を保存し、以下のコマンドを実行
```
$ python PrepareChain.py
```

### 文章の生成
事前準備がされていることが前提
```
$ python GenerateText.py
```
生成する文章の数を引数で指定可能(省略した場合は1)
```
$ python GenerateText.py 5
```

## 各ファイル
### README.md
このファイル

### PrepareChain.py
適当なテキストを与えて、そこから3つ組のチェーンを作成し、DBに保存するファイル

### schema.sql
DB作成のためのスキーマファイル

### GenerateText.py
実際にランダムで文章を生成するファイル

### chain.db
gitで管理はされていないが、3つ組チェーンの情報が保存されているDBファイル

### text.txt
元になる文章