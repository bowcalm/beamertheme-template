# beamertheme-template

## 概要

Beamerをカスタムするためのテンプレート。カスタム可能なオブジェクトは[BEAMER appearance cheat sheet](http://www.cpt.univ-mrs.fr/~masson/latex/Beamer-appearance-cheat-sheet.pdf)を参照してください。

## Beamer's Fonts

フォントスタイル「xxx」のファイル名は「beamerfontthemexxx.sty」である必要があります。  
フォントは`setbeamerfont`コマンドによって指定します。  
詳しくは[こちら](https://ftp.kddilabs.jp/CTAN/macros/latex/contrib/beamer/doc/beameruserguide.pdf#page=202)を参照してください。

```sty
\setbeamerfont{"some beamer object"}{
  family = "family command",
  series = "series command",
  shape = "shape command",
  size = "size command",
  parent = "inherited objects"
}
```

使用例は以下の通り。

```sty
\setbeamerfont{title}{
  family = \sffamily,
  series = \bfseries,
  shape = \upshape,
  size = \large,
  parent = {structure, palette primary}
}
```

## Beamer's Colors

カラースタイル「xxx」のファイル名は「beamercolorthemexxx.sty」である必要があります。  
カラーは`setbeamercolor`コマンドによって指定します。  
詳しくは[こちら](https://ftp.kddilabs.jp/CTAN/macros/latex/contrib/beamer/doc/beameruserguide.pdf#page=188)を参照してください。

```sty
\setbeamercolor{"some beamer object"}{
  fg = "some color",
  bg = "some color",
  parent = "inherited objects",
  use = "referenced objects"
}
```

使用例は以下の通り。

```sty
\setbeamercolor{title}{
  fg = red!50!structure.fg,
  bg = green!70!palette primary.bg,
  parent = palette primary,
  use = {structure, palette primary}
}
```
