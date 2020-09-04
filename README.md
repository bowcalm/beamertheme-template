# beamertheme-template

## Overview

This is a template for customizing Beamer. Objects that can be customized refer to [BEAMER appearance cheat sheet](http://www.cpt.univ-mrs.fr/~masson/latex/Beamer-appearance-cheat-sheet.pdf).

## Beamer's Fonts

The filename of the font style "xxx" must be "beamerfontthemexxx.sty".  
Specify the font using the `setbeamerfont` command.  
Please check [here](https://ftp.kddilabs.jp/CTAN/macros/latex/contrib/beamer/doc/beameruserguide.pdf#page=202) for more details.

```sty
\setbeamerfont{"some beamer object"}{
  family = "family command",
  series = "series command",
  shape = "shape command",
  size = "size command",
  parent = "inherited objects"
}
```

An example of use is as follows.

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

The filename of the color style "xxx" must be "beamercolorthemexxx.sty".  
Specify the color using the `setbeamercolor` command.  
Please check [here](https://ftp.kddilabs.jp/CTAN/macros/latex/contrib/beamer/doc/beameruserguide.pdf#page=188) for more details.

```sty
\setbeamercolor{"some beamer object"}{
  fg = "some color",
  bg = "some color",
  parent = "inherited objects",
  use = "referenced objects"
}
```

An example of use is as follows.

```sty
\setbeamercolor{title}{
  fg = red!50!structure.fg,
  bg = green!70!palette primary.bg,
  parent = palette primary,
  use = {structure, palette primary}
}
```
