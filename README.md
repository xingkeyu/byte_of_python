# A Byte of Python

## 安装

确保已经安装了Python 2.7 或更高版本。

从<http://johnmacfarlane.net/pandoc/installing.html>安装Pandoc。

从<http://www.tug.org/texlive/>安装pdflatex。
注意：Mac用户可从<http://www.tug.org/mactex/2012/>安装`MacTex.pkg`。

如果没安装`pip`，请安装：

    sudo sh -c "curl -k -O https://raw.github.com/pypa/pip/master/contrib/get-pip.py && python get-pip.py && rm get-pip.py"


安装需要的Python库：

    sudo pip install -r requirements.txt


将源文件转换为HTML文件：

    fab html

将源文件转换为PDF文件:

    fab pdf

将源文件转换为EPUB (电子书)文件:

    fab epub

## 编辑

如果你使用 Vim 编辑器，那么或许你会喜欢 [vim-pandoc](https://github.com/vim-pandoc/vim-pandoc) 插件。但是对大文章它有一个缺点，变得确实很慢。因此，我只在纯文本模式(`:set ft=`)下编辑，在`pandoc`(`:set ft=pandoc`)模式下检查。
