#简单搭建Hexo博客<br>
##前言<br>
其实我一开想学习Hexo不是因为想在github搭建自己的Hexo博客，而是想在学习Hexo读取Markdown文件的方法，但是我发现Hexo的实现原理还是有点复杂的，所以我就先搭建一下，慢慢再去学习这个。[Hexo官网](https://hexo.io/)其实有很详细的教程，那么我就简单的小结一下。<br>
##搭建步骤<br>
####需要的工具<br>
npm<br>
Git(下载主题，或者是将hexo设置称自己的github静态网站也是需要的)<br>
####步骤<br>
在cmd执行一下命令安装hexo-cli插件
```
$ npm install -g hexo-cli
```

然后就是在cmd执行以下命令完成安装和初始化项目
```
$ hexo init <folder> //初始化folder
$ cd <folder> 
$ npm install //下载需要的插件
```

启动项目，在浏览器打开http://localhost:4000/
```
hexo server
```


####更换主题<br>
使用git将主题下载到themes目录
```
$ git clone https://github.com/theme-next/hexo-theme-next themes<br>ext
```
然后在根目录的_config.yml文件将“theme: landscape” 修改成“theme: next”，不要忘记next前面有空格<br>
最后重新启动项目，就可以了。<br>
