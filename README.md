# vim_file_info
vim 一键自动 添加文件作者信息 添加宏定义</br>
步骤：</br>
1.安装NERD_commenter.vim(cp doc/  ~/.vim  cp plugin/  ~/.vim )</br>
2.将authorinfo.vim下载后放到plugin目录下（cp authorinfo.vim  ~/.vim/plugin/）</br>
3. 将head_def.vim下载后放到plugin目录下（cp head_def.vim  ~/.vim/plugin/）</br>
4.在vimrc中进行如下配置:</br>
let g:vimrc_author='Daniel' </br>
let g:vimrc_email='***@gmail.com' </br>
let g:vimrc_homepage='http://www.vimer.cn' </br>

nmap <F4> :AuthorInfoDetect<cr> </br>
nmap ,ha :call InsertHeadDefN()<CR></br>


当在normal模式按下,F4 就会插入头文件。</br>

当在normal模式按下,ha，就会先匹配/*..*/这样的组合，如果匹配成功的话，就会在*/后插入</br> 宏定义，如果匹配不成功的话，就会在一开始插入宏定义。</br>

参考：</br>
1,http://www.vimer.cn/2011/02/vimgvim%e6%b7%bb%e5%8a%a0%e4%bd%9c%e8%80%85%e4%bf%a1%e6%81%af%e6%8f%92%e4%bb%b6%e5%8d%87%e7%ba%a7%e7%89%88-%e6%9b%b4%e6%99%ba%e8%83%bd%e6%94%af%e6%8c%81%e6%9b%b4%e5%a4%9a%e8%af%ad%e8%a8%80.html
</br>
2,http://www.vimer.cn/2010/01/%e7%94%a8vim%e5%9c%a8%e4%bb%a3%e7%a0%81%e6%96%87%e4%bb%b6%e4%b8%ad%e8%87%aa%e5%8a%a8%e6%b7%bb%e5%8a%a0ifdefdefineendif.html
