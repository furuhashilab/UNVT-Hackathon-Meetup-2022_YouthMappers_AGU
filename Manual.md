## Produce編

## 必須ソフト
[homebrew](https://qiita.com/zaburo/items/29fe23c1ceb6056109fd)

[nodebrew](https://qiita.com/fuqda/items/1b780d7e0658fb7a3889)

[Tippecanoe](https://github.com/mapbox/tippecanoe)

[QGIS](https://qgis.org/ja/site/forusers/download.html)

## homebrew インストール方法
↓このコマンドをそのままターミナルで入力(入力する前に```cd```と入力してホームディレクトリにあることを確認)

```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```


<img width="565" alt="homebrew インストール" src="https://user-images.githubusercontent.com/40018527/146682170-cc09d51c-f99a-4446-bd61-2ba3d13fb28a.png">

Passwordの部分はPC起動時に入力するパスワードを入力


## nodebrew　インストール方法
↓このコマンドをそのままターミナルで入力(入力する前に```cd```と入力してホームディレクトリにあることを確認)

```curl -L git.io/nodebrew | perl - setup```


<img width="564" alt="nodebrewダウンロード" src="https://user-images.githubusercontent.com/40018527/146682369-455ab7c8-7e20-4bea-896c-fc43b766fa25.png">


## Tippecanoeインストール方法

↓このコマンドを順番に入力する(4行目からは%以降を入力すること）

```cd```

```git clone https://github.com/mapbox/tippecanoe```

```cd tippecanoe```

```[tippecanoe] % make -j```

```[tippecanoe] % sudo make install```

