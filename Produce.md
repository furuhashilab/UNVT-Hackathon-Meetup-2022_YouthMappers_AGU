# Produce編 / Produce

## 必須ソフト / Necessary softwares

[homebrew](https://qiita.com/zaburo/items/29fe23c1ceb6056109fd)

[nodebrew](https://qiita.com/fuqda/items/1b780d7e0658fb7a3889)

[Tippecanoe](https://github.com/mapbox/tippecanoe)

[QGIS](https://qgis.org/ja/site/forusers/download.html)

## homebrew インストール方法 / How to install homebrew

↓このコマンドをそのままターミナルで入力(入力する前に```cd```と入力してホームディレクトリにあることを確認)

↓type this command into terminal (before you type the command, type ```cd``` and make sure you are in home ditectory)

<br>
<br>

```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```


<img width="565" alt="homebrew インストール" src="https://user-images.githubusercontent.com/40018527/146682170-cc09d51c-f99a-4446-bd61-2ba3d13fb28a.png">

Passwordの部分はPC起動時に入力するパスワードを入力

type your password when you start your PC in the password field

<br>
<br>

## nodebrew　インストール方法 / How to install nodebrew

↓このコマンドをそのままターミナルで入力(入力する前に```cd```と入力してホームディレクトリにあることを確認)

↓type this command into terminal (before you type the command, type ```cd``` and make sure you are in home ditectory)

<br>
<br>

```curl -L git.io/nodebrew | perl - setup```


<img width="564" alt="nodebrewダウンロード" src="https://user-images.githubusercontent.com/40018527/146682369-455ab7c8-7e20-4bea-896c-fc43b766fa25.png">

<br>
<br>

## Tippecanoeインストール方法 / How to install Tippecanoe

↓このコマンドを順番に入力する(4行目からは%以降を入力すること）

↓type this command in order (after the fourth line, just type after the %)

<br>
<br>

```cd```

```git clone https://github.com/mapbox/tippecanoe```

```cd tippecanoe```

```[tippecanoe] % make -j```

```[tippecanoe] % sudo make install```

↑これでインストールできない場合

g++とlibsqlite3をインストール

<br>
<br>

↑if you can't install with this,

install g++ and libsqlite3

<br>
<br>

```sudo apt install build-essential```

```sudo apt install libsqlite3-dev zlib1g-dev```

<br>
<br>

## GeoJSONをTippecanoeを使ってPbf化 / Convert GeoJASON to Pbf using Tippecanoe

↓このコマンドをそのままターミナルで入力(入力する前に```cd```と入力してホームディレクトリにあることを確認)

↓(workspace)にはproduceするデータのファイルが存在する階層名、(filename)にはそのファイル名、

 (dataname)には該当する個々のデータ名　を入力
 
 <br>
 <br>

↓type this command into Tippecanoe

 (before you type the command, type ```cd``` and make sure you are in home ditectory)

 in (workspace), type the name of the place where the data file to be produced exists
 
 in (filename), type the name of the data file
 
 in (dataname), type the name of the individual relevant data

<br>
<br>

```cd```

```cd (workspace)/(filename)```

```tippecanoe --no-tile-compression -z23 -Z12 -e (dataname) -y code -l layername -ai (dataname).geojson```

![1](https://user-images.githubusercontent.com/72395572/146860311-5bba8e2d-5ac7-4ad9-85e7-d77c847f7fd5.jpg)

これで一つのデータのPbf化が完了

残りの該当データの数だけ、上記の工程を繰り返す

<br>
<br>

this is the end of the converting of one piece of data

repeat the above process for the remaining data

![3](https://user-images.githubusercontent.com/72395572/146861268-e527b3bd-bba5-428f-97d7-58e94778b966.jpg)

これでTippecanoeを用いてGeoJASONをPbf化する工程の完了

this is the end of the process of converting GeoJASON to Pbf using Tippecanoe


















