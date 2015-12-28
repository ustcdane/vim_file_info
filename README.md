# vim_file_info
vim 一键自动 添加文件作者信息  代码文件中自动添加#ifdef,#define,#endif的头文件宏定义 </br>
步骤：</br>
1.安装NERD_commenter.vim(cp -r nerdcommenter/doc  &nbsp ~/.vim ; 
cp   plugin/NERD_commenter.vim     ~/.vim/plugin )</br>
2.将authorinfo.vim下载后放到plugin目录下（cp authorinfo.vim  ~/.vim/plugin/）</br>
3. 将head_def.vim下载后放到plugin目录下（cp head_def.vim  ~/.vim/plugin/）</br>
4.在vimrc中进行如下配置:</br>
> let g:vimrc_author='Daniel' </br>
> let g:vimrc_email='***@gmail.com' </br>
> let g:vimrc_homepage='http://ustcdane.github.io/' </br>
> nmap <F4> :AuthorInfoDetect<cr> </br>
> nmap ,ha :call InsertHeadDefN()<cr>

当在normal模式按下,F4 就会插入头文件。</br>

当在normal模式按下,ha，就会先匹配/*..*/这样的组合，如果匹配成功的话，就会在*/后插入</br> 宏定义，如果匹配不成功的话，就会在一开始插入宏定义。</br>
</br>
viminstall.tar.gz
用vim的插件搭建一个类似sourceinsight的vi，同时加了一些vim及脚本，只需一条命令，就可安装完ctagslist,cscope等插件，达到sourceinsight的效果。
</br>说明见：</br>
http://blog.csdn.net/daniel_ustc/article/details/8299096


参考：</br>
1,http://www.vimer.cn/2011/02/vimgvim%e6%b7%bb%e5%8a%a0%e4%bd%9c%e8%80%85%e4%bf%a1%e6%81%af%e6%8f%92%e4%bb%b6%e5%8d%87%e7%ba%a7%e7%89%88-%e6%9b%b4%e6%99%ba%e8%83%bd%e6%94%af%e6%8c%81%e6%9b%b4%e5%a4%9a%e8%af%ad%e8%a8%80.html
</br>
http://www.vimer.cn/2010/01/%E7%94%A8vim%E5%9C%A8%E4%BB%A3%E7%A0%81%E6%96%87%E4%BB%B6%E4%B8%AD%E8%87%AA%E5%8A%A8%E6%B7%BB%E5%8A%A0ifdefdefineendif.html</br>
2,http://www.vimer.cn/2010/01/%e7%94%a8vim%e5%9c%a8%e4%bb%a3%e7%a0%81%e6%96%87%e4%bb%b6%e4%b8%ad%e8%87%aa%e5%8a%a8%e6%b7%bb%e5%8a%a0ifdefdefineendif.html </br>
3,http://www.vimer.cn/2010/06/%e6%9c%ac%e5%8d%9a%e4%bd%bf%e7%94%a8%e7%9a%84vimgvim%e7%9b%b8%e5%85%b3%e6%8f%92%e4%bb%b6%e6%95%b4%e7%90%86.html  </br>
4, 发现一个配置vim不错的网址，mark：https://github.com/wklken/k-vim
