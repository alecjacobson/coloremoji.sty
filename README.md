coloremoji.sty
==============
Style package for directly including color emojis in latex documents

Installation

    mkdir -p ~/Library/texmf/tex/latex/local
    cd ~/Library/texmf/tex/latex/local
    git clone git@github.com:alecjacobson/coloremoji.sty.git
    texhash coloremoji.sty

[Related blog entry](http://www.alecjacobson.com/weblog/?p=4018)

## Examples

The following LaTeX code:

    \documentclass{article}
    \usepackage{coloremoji}
    \begin{document}
    Hello, 🌎.
    \end{document}

produces something like:

![Hello, world.](http://alecjacobson.com/weblog/media/hello-world-emoji.png)

You can even use emojis in math. The following LaTeX code:

    \[
    🐊^{🐊^{🐊}} = ∫_{🎃} 🙊 \ d🍀
    \]

produces something like:

![Emojis in math
mode.](http://alecjacobson.com/weblog/media/alligator-power-integral-jack-o-lantern.png)

## Known issues

This style sheet creates a PDF where each emoji is actually an embedded _image_
rather than a character using the [Apple Color Emoji
typeface](http://en.wikipedia.org/wiki/Apple_Color_Emoji). This means you won't
be able to correctly copy and paste emjois from the resulting .pdf files.

The encoding of the `.tex` must support emoji's, that is unicode characters. So switch your encoding to something like UTF-8.
