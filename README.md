ln ~/lucky-vim/vimrc ~/.vimrc
ln ~/lucky-vim/vimrc.bundles ~/.vimrc.bundles
git checkout <file>底层操作应该是：
 1:rm <file>
 2:把.git里的<file> 复制到当前位置
所以ln 后执行checkout会让连接数变为一，因为原来的那个文件已经删除了
