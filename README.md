# A Byte of Python

## 安装

确保已经安装Python (&gt;= 2.7)。

从<http://johnmacfarlane.net/pandoc/installing.html> 安装 Pandoc。

从 <http://www.tug.org/texlive/> 安装　pdflatex。
注意：Mac用户可从<http://www.tug.org/mactex/2012/>安装 `MacTex.pkg` 。

如果没安装 `pip` 请安装：

    sudo sh -c "curl -k -O https://raw.github.com/pypa/pip/master/contrib/get-pip.py && python get-pip.py && rm get-pip.py"


安装需要的 Python 库：

    sudo pip install -r requirements.txt


将源文件转换为 HTML 文件：

    fab html

将源文件转换为 PDF 文件:

    fab pdf

将源文件转换为 EPUB (电子书)文件:

    fab epub

## 编辑

如果你使用 Vim 编辑器，那么或许你会喜欢 [vim-pandoc](https://github.com/vim-pandoc/vim-pandoc) 插件。There is one downside though - for long chapters, it becomes really slow, so I edit only in plain text mode (`:set ft=`), but when reviewing, I use the `pandoc` (`:set ft=pandoc`) mode.
