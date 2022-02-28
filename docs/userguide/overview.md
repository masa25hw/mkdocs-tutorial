# User Guide

## 基本操作

### プロジェクトの新規作成(mkdocs new)
```bash
mkdocs new <project name>
```

### ドキュメントサーバの起動(mkdocs serve)
```bash
mkdocs serve
```

サーバを停止する場合は`Ctrl + C`を入力する。

サーバ起動後、`http://127.0.0.1:8000/mkdocs-tutorial/`にアクセスすることで生成内容を確認できる。

### デプロイ用コンテンツの作成(mkdocs build)
```bash
mkdocs build
```

「site」ディレクトリとともに配下に静的コンテンツが生成される。生成されたコンテンツを任意のWebサーバなどにデプロイすれば完成。`--clean`オプションを付けて実行することで「site」配下の古いファイルを削除した上で作成できる。

ページはMarkdownファイル(*.md)として作成し、Markdown形式またはHTML形式での記載内容を認識・表示する。

サーバを起動させたまま編集・保存を行うことも可能なので、保存後にリアルたアイムで編集内容がhン営されて確認もスムーズに行うことができる。

## MkDocksの設定

### サイト名の変更
`site_name`でドキュメントサイトの名称を指定できる。
```
site_name: MkDocs Tutorial
```
### ベースドキュメントフォルダの指定
`docs_dir`で任意のドキュメントルートフォルダを指定することができる。（初期設定は`docs`）

```
docs_dir: 'docs'
```

### Copyrightの指定
`copyright`で著作権情報に関する記載を指定できる。

```
copyright: 'Copyright © 2010 - 2022 - Hogehoge, Inc.'
```

### テーマに関する設定
`theme`でMkDocsの表示スタイルに関する設定を行うことができる。

```
theme:
    name: material
    language: ja
    icon:
        logo: material/school
        repo: fontawesome/brands/git-alt
    favicon: favicon.png
    # タブ表示を有効.
    features:
        - tabs
```

#### 言語指定
検索インデックスを構築する時に使用する言語を指定。
```
language: ja
```

#### アイコン指定
サイト名と併せて表示されているアイコン画像を個別に指定可能。

```
icon:
    logo: material/school
    repo: fontawesome/brands/git-alt
```

#### Favicon指定
任意の画像を用意し、faviconでその画像を指定することでfaviconとして表示させることができる。(docsをルートとするパス指定)

### タブ形式のメニュー表示
`theme`配下に以下の形で設定を追記することで、メニュー構成を「タブ配置を踏まえた」形に変更することが出来ます(後述する`nav`の1階層目をタブで切り替えできるようにするオプション)。