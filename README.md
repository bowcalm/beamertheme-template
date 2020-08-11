# beamertheme-template

## Overview

This is a template for customizing Beamer. Elements that can be customized refer to [BEAMER appearance cheat sheet](http://www.cpt.univ-mrs.fr/~masson/latex/Beamer-appearance-cheat-sheet.pdf).

## Beamer's Colors

The filename of the color style "xxx" must be "beamercolorthemexxx.sty".  
Specify the color using the `setbeamercolor` command. Perhaps "fg" means foreground and "bg" means background.

### Command definition

```sty
\setbeamercolor*{"some beamer element"}{
  fg = "some color",
  bg = "some color"
}
```

### Example

```sty
\setbeamercolor*{title}{
  fg = red,
  bg = green
}
```
