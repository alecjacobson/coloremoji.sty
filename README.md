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

Produces something like:

![Hello, world.](http://alecjacobson.com/weblog/media/hello-world-emoji.png)
