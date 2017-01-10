Paper(less)Color Theme
===================

*Note*: The current document has not been updated for the current stage of the project. Some information apply only for version 0.7 and earlier.

Light & Dark color schemes for **Vim** terminal editor and **gVim**

Inspired by Google's Material Design

**Now with less syntax highlighting!**

Improve code readability; great for presentation

Currently designed for these file types:  C, C++, Java, Makefile, CMake, Lex/Flex & Yacc/Bison, Bash, VimL, Golang, JavaScript, JSON, HTML, XML, Python, Ruby, Markdown, DTrace, SystemTap, PlantUML, Haskell, Assembly (MIPS, GAS, NASM), SQL/MySQL, Octave/MATLAB, Fortran, R, Pascal, PHP, Perl, LUA, Clojure, Dockerfile, NGINX, Yaml, Dosini, Mail, reStructuredText, Erlang, Elixir, Cucumber

Other file types can still display well as long as your Vim is set up to recognize the language syntax even though that may not be the optimal experience. So, if the language you are working on isn't listed here, feel free to make a design request.

Plugin support: vimdiff, netrw, [NERDTree](https://github.com/scrooloose/nerdtree), [tagbar](https://github.com/majutsushi/tagbar), [tabline](https://github.com/mkitt/tabline.vim), [vim-airline](https://github.com/bling/vim-airline), [vim-indent-guides](https://github.com/nathanaelkane/vim-indent-guides), [vim-startify](https://github.com/mhinz/vim-startify)

(see below for syntax-highlighting plugins target)

## Installation
Place 'PaperlessColor.vim' file into 'colors' folder within your Vim directory, e.g. `~/.vim/colors/`

Or simply use a plugin manager like [Plug](https://github.com/junegunn/vim-plug) (recommended for easy `:PlugUpdate`):

    Plug 'duckwork/paperlesscolor-theme'

Then, put this in your `~/.vimrc`

```VimL
set t_Co=256   " This is may or may not needed.

set background=light
colorscheme paperlesscolor
```

Or using the dark version: 

```VimL
set background=dark
colorscheme paperlesscolor
```

To switch to dark or light variant during session: `:set background=dark` or `:set background=light`

To quickly toggle between them, use [vim-unimpaired](https://github.com/tpope/vim-unimpaired)'s keymap `cob`

*Optional*: turn on line numbers and status bar

```VimL
set number
set laststatus=2
```

## Highlighting Customization

Some elements have default highlighting color that may not fit everyone, and you can customize their HEX color code in your .vimrc file.
Refer to 256-color table when choosing color.

Example of currently available options:

```VimL
let g:PaperColor_Dark_Override = { 'background' : '#1c1c1c', 'cursorline' : '#abcdef', 'matchparen' : '#3a3a3a', 'comment' : '#5f875f' }

let g:PaperColor_Light_Override = { 'background' : '#abcdef', 'cursorline' : '#dfdfff', 'matchparen' : '#d6d6d6' , 'comment' : '#8e908c' }
```

## Syntax Highlighting Plugins Target
There are syntax highlighting enhancement plugins that improve upon Vim built-in syntax highlighting, and each can have many different implementations. This is the list of plugins that this color scheme targets.

* C: [c-syntax.vim](https://github.com/NLKNguyen/c-syntax.vim)
* JavaScript: [vim-javascript](https://github.com/pangloss/vim-javascript)
* JSON: [vim-json](https://github.com/elzr/vim-json)
* Go: [vim-go](https://github.com/fatih/vim-go)
* DTrace: [dtrace-syntax-file](https://github.com/vim-scripts/dtrace-syntax-file)
* SystemTap: [vim-systemtap](https://github.com/nickhutchinson/vim-systemtap)
* Haskell: [haskell-vim](https://github.com/raichoo/haskell-vim)
* PlantUML: [plantuml-syntax](https://github.com/aklt/plantuml-syntax)
* Markdown: [vim-markdown](https://github.com/plasticboy/vim-markdown)
* Assembly MIPS: [mips](https://github.com/vim-scripts/mips.vim)
* Assembly GAS: [vim-gas](https://github.com/Shirk/vim-gas)
* Octave/MATLAB: [vim-octave](https://github.com/jvirtanen/vim-octave)
* Python: [python-syntax](https://github.com/hdima/python-syntax/)
* Dockerfile: [dockerfile.vim](https://github.com/docker/docker/tree/master/contrib/syntax/vim)
* NGINX: [nginx-vim-syntax](https://github.com/evanmiller/nginx-vim-syntax)
* Elixir: [vim-elixir](https://github.com/elixir-lang/vim-elixir)


## Screenshots

_We ain't got none of them fancy screenshots!_

For more sceenshots, story behind the project, and other users' designs inspired by Paper Color, go to [this blog post](http://nlknguyen.com/2015/05/21/vim-paper-color-theme/)

Suggestions/Wishes/Questions/Comments are welcome via [Github issues](https://github.com/NLKNguyen/papercolor-theme/issues) or via the blog above.

# Related Projects Based On Paper(Less)Color
The original [PaperColor](http://github.com/NLKNguyen/papercolor-theme) project is a great colorscheme, but I want fewer highlight groups.  Thus, Paper(Less)Color.
