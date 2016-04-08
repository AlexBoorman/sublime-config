#Sublime Text 3 Configuration

##Requisites

+ Package Control <br>
    [http://packagecontrol.io](https://packagecontrol.io/)

+ NodeJS <br>
    [http://nodejs.org](https://nodejs.org/en/)

+ Homebrew <br>
    [http://brew.sh](http://brew.sh)

+ Composer <br>
    [http://getcomposer.org](https://getcomposer.org/download/)

+ PHP 5.4.4+ <br>
    [http://php.net](http://php.net/)

+ MySQL 5.5.37+ <br>
    [http://dev.mysql.com](http://dev.mysql.com/doc/refman/5.5/en/)


---------------------------------------
##Terminal Use

    CREATE sublime SYMLINK OR ALIAS FOR THE TERMINAL
<br>
**SymLink:**

    sudo ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/bin/sublime
<br>
**Alias:** `~/.bash_profile`

    alias sublime='open -a "Sublime Text"'


---------------------------------------
##Package Control

[http://packagecontrol.io](https://packagecontrol.io/)

`Paste into the console and hit return`

    import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

---------------------------------------
##Core Packages

    Emmet
    SideBarEnhancements
    BracketHighlighter
    SublimeCodeIntel
    Alignment
    Modific
    ColorPicker
    HTML-CSS-JS Prettify
    Color Highlighter
    Style Sorter
    TrailingSpaces
    AutoPrefixer
    ChangeQuotes
    
    EditorConfig -  http://editorconfig.org
    Function Name Display
    Date Formatter
    DocBlockr
    Inc-Dec-Value
    phpfmt
    Markdown Preview
    
    


###Emmet / [Docs](http://docs.emmet.io/) - [CheatSheet](http://docs.emmet.io/cheat-sheet/)

    Speeds up HTML & CSS workflow with text expansion, regex, snippets and tab completion

###SideBarEnhancements

    Enhancements to the sidebar, files and folders

###BracketHighlighter

    Bracket and tag highlighter for Sublime Text

###SublimeCodeIntel / [Docs](http://sublimecodeintel.github.io/SublimeCodeIntel/)

    Full-featured code intelligence and smart autocomplete engine


###Alignment

    Easy alignment of multiple selections and multi-line selections

MAC

    ⌘ + ^ + a

LINUX

    ctrl + alt + a

###Modific / [Docs](https://packagecontrol.io/packages/Modific)

    Highlight lines changed since the last commit (supports Git, SVN, Bazaar, Mercurial and TFS) / ST2(3) plugin.
    
**SHOW DIFF**
    
    ctrl + alt + d  

**PREVIEW COMMIT FOR CURRENT LINE**


###ColorPicker / [Docs](https://packagecontrol.io/packages/ColorPicker)

    Use OS native color picker in Sublime Text

MAC

    ⌘ + shift + c

LINUX / WINDOWS

    ctrl + shift + c

###HTML-CSS-JS Prettify /  [Docs](https://github.com/victorporof/Sublime-HTMLPrettify)
`REQUIRES NODE.JS & JS-BEAUTIFY`



    Runs prettify on HTML, CSS, JS & JSON

**BEAUTIFY OPEN FILE OR SELECTION**

MAC

    ⌘ + shift + h

LINUX

    ctrl + shift + h

**BEAUTIFY ON SAVE**

1. Open the command palette

2. Type `htmlprettify`

3. Select `Plugin Options`

4. Set `format_on_save` to `true`

###Color Highlighter

    Highlights inline colors (HEX, RGBA) with their actual color

###Style Sorter

    Auto sorts CSS style properties uniformly

###TrailingSpaces

    Purges page of trailing spaces, which can cause JS errors, on save

###AutoPrefixer
`REQUIRES NODE.JS`

    Sublime plugin to  add vendor prefixes to your CSS

###ChangeQuotes

    Converts single to double / double to single quotes, preserves escaping


##SublimeLinter 3 / [Docs](http://www.sublimelinter.com/en/latest/)

Interactive code linting framework for Sublime Text 3

###SublimeLinter-php

    PHP linter using php-l

###SublimeLinter-phplint / [Docs](https://packagecontrol.io/packages/SublimeLinter-phplint) - [Site](http://www.icosaedro.it/phplint/index.html)

    PHP linter using phplint

**MAC** 

    brew install homebrew/php/phplint


###SublimeLinter-phpmd / [Docs](https://packagecontrol.io/packages/SublimeLinter-phpmd) - [Site](https://phpmd.org/documentation/index.html)

    PHP linter using phpmd

###SublimeLinter-phpcs / [Docs](https://packagecontrol.io/packages/SublimeLinter-phpcs) - [Site](http://pear.php.net/package/PHP_CodeSniffer/)

    PHP linter using phpcs

###SublimeLinter-jshint / [Docs](https://packagecontrol.io/packages/SublimeLinter-jshint) - [Site](http://www.jshint.com/docs/)

    JS linter using jshint

<br>
**INSTALL WITH NPM** 
    
    npm install -g jshint


###SublimeLinter-json / [Docs](https://packagecontrol.io/packages/SublimeLinter-json)

    JSON linter using Sublime Text's JSON Parser

###SublimeLinter-csslint / [Docs](https://packagecontrol.io/packages/SublimeLinter-csslint) - [Site](https://github.com/stubbornella/csslint/wiki)

    CSS linter using csslint

**INSTALL WITH NPM** 

    npm install -g csslint

###SublimeLinter-html-tidy / [Docs](https://packagecontrol.io/packages/SublimeLinter-html-tidy) - [Site](http://www.html-tidy.org/)

    HTML linter using html-tidy (html4 or html5)


**MAC** 

        brew install tidy-html5
    
**LINUX** (HTML5 REQUIRES BUILD)

    apt-get install tidy
    

**WINDOWS**

    Windows binaries are available for both html4 and html5


###phpfmt / [Docs](https://packagecontrol.io/packages/phpfmt/) - [Site](https://github.com/phpfmt/fmt)

    PSR1/PSR2 PHP Code Formatter

###Languages, Snippets & Bundles

    HTML5
    CSS3
    IconFont
    MarkDown Editing
    Markdown Extended
    php-snippets
    Bootstrap 3
    Bootstrap 3 Snippets
    Jade
    Haml
    GenericConfig
    Nginx
    ApacheConf.tmLanguage
    Babel
    Better CoffeeScript
    Dockerfile Syntax Highlighting
    Dotfiles Syntax Highlighting
    Hosts
    PHP MySQLi Connection
    jQuery
    JQuery Snippets
    SASS
    LESS
    Emmet CSS Snippets
    Comment Snippets


###Color Schemes & Themes

    Monokai Extended
    MonokaiJSON+
    Monokai Neue
    Materialize
    Spacegray
    
    
###User Settings Configuration

    {
    "bold_folder_labels": true,
    "color_scheme": "Packages/Monokai Extended/Monokai Extended Light.tmTheme",
    "font_face": "Droid Sans Mono",
    "font_options": "subpixel_antialias",
    "font_size": 13,
    "highlight_line": true,
    "highlight_modified_tabs": true,
    "ignored_packages":
    [
        "Vintage"
    ],
    "line_padding_bottom": 1,
    "line_padding_top": 1,
    "rulers":
    [
        80
    ],
    "scroll_past_end": true,
    "tab_size": 4,
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true,
    "word_wrap": true
    }
    
