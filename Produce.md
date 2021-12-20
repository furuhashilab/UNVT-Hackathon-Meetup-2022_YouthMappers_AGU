# 日本語

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

↑これでインストールできない場合

g++とlibsqlite3をインストール

```sudo apt install build-essential```

```sudo apt install libsqlite3-dev zlib1g-dev```


##　GeoJSONをTippecanoeを使ってMbtile化
↓Tippecanoeで入力するコマンド

# English

## First step: Produce

## Necessary software

[homebrew](https://qiita.com/zaburo/items/29fe23c1ceb6056109fd)

[nodebrew](https://qiita.com/fuqda/items/1b780d7e0658fb7a3889)

[Tippecanoe](https://github.com/mapbox/tippecanoe)

[QGIS](https://qgis.org/ja/site/forusers/download.html)

## How to install homebrew
↓type this command into terminal (before you type the command, type ```cd``` and make sure you are in home ditectory)

```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```


<img width="565" alt="homebrew インストール" src="https://user-images.githubusercontent.com/40018527/146682170-cc09d51c-f99a-4446-bd61-2ba3d13fb28a.png">

type your password when you start your PC in the password field


## How to install nodebrew
↓type this command into terminal (before you type the command, type ```cd``` and make sure you are in home ditectory)


```curl -L git.io/nodebrew | perl - setup```


<img width="564" alt="nodebrewダウンロード" src="https://user-images.githubusercontent.com/40018527/146682369-455ab7c8-7e20-4bea-896c-fc43b766fa25.png">


## How to install Tippecanoe

↓type this command in order (after the fourth line, just type after the %)

```cd```

```git clone https://github.com/mapbox/tippecanoe```

```cd tippecanoe```

```[tippecanoe] % make -j```

```[tippecanoe] % sudo make install```

↑if you can't install with this,

install g++ and libsqlite3


```sudo apt install build-essential```

```sudo apt install libsqlite3-dev zlib1g-dev```


## Convert GeoJASON to Mbtile using Tippecanoe
↓type this command into Tippecanoe

