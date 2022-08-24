需要拷贝的文件如下：
autoload,vim82下没有autoload文件，直接拷贝过去；
doc,将doc下的所有文件拷贝到vim82/doc文件下；
plugin,将plugin下的所有文件拷贝到vim82/plugin文件下；
lib,将lib文件直接拷贝过去；
nerdtree_plugin，将nerdtree_plugin文件直接拷贝过去。

打开git安装路径：git/etc,找到vimrc文件
打开vimrc文件，在文件末尾添加：
" 打开vim时,自动打开NERDTree
autocmd vimenter * NERDTree

" 设置NerdTree打开的快捷键,可自行更改
map <F2> :NERDTreeMirror<CR>
map <F2> :NERDTreeToggle<CR>
