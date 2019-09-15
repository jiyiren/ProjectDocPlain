<p>
    <a href="https://jiyiren.github.io/"><img alt="logo" width="40" height="40" src="http://img.godjiyi.cn/jiyiheaderh-icon.png" alt="jiyiren">
    </a>
</p>

<p align="center" style="font-size: 2em">
    基于 Gitbook 的项目文档设计
</p>

<p align="center" style="font-size: 16px">@<a href="https://jiyiren.github.io/">JIYI</a> @<a href="https://jiyiren.github.io/">Leader</a> @<a href="https://jiyiren.github.io/">Boss</a></p>

<p align="center" style="margin: 30px 0 35px;">基于 Gitbook 的开源生态，更具美观的项目文档库</p>


此系统主要面向于 **IT 项目开发者** 服务。作者集成了一些必要的插件以及一些规范化的写作风格，整体上以简洁、清晰为主要设计倾向。本项目基于 **Gitbook** 开源生态，具有较多开源插件、模板支持，使用性较广，问题排查方便，且可导出为 `HTML`、`PDF` 等格式传播，形式多样。也具有 `Book`、`API`、`FQA` 等多种模式形态，丰富实用。此文档基于个人审美自定义的，大家可以根据自身感觉进行重新设计扩展。公司内部文档应放在公司的 **[Gitlab](https://www.gitlab.com/)** 里，个人的可以放 **[Github](https://www.github.com/)** 中以 **Pages** 方式开放。

![](http://img.godjiyi.cn/jy_projectdocbg.jpg)

## 目录内容

本文档包含以下内容(**均是示例**)：

- [基本环境](#基本环境)
	- [安装 Nodejs](安装-nodejs)
	- [安装 gitbook](安装-gitbook)
	- [使用 gitbook](使用-gitbook) 
- [参考链接](#参考链接)


# 基本环境

## 安装 Nodejs
	
* 全球官网：[https://nodejs.org/en](https://nodejs.org/en)
* 中文官网：[http://nodejs.cn/](http://nodejs.cn/)
	
下载安装后测试下 Node 是否安装成功：
	
```bash
$ node -v
v10.15.3
```
	
如果提示命令没找到，那么是由于 Node 没有加入环境变量，大家将安装的 Node 环境地址放在环境变量里就可以了。

## 安装 gitbook

直接输入命令进行安装：
	
```bash
$ npm install gitbook-cli -g
```
	
`npm` 也是和 `node` 一起安装的，`node` 存在 `npm` 就存在。`-g` 参数表示全局安装，也就是模块包会安装到全局环境里，这个是推荐做法，因为像这种工具命令全局安装是最好的。而项目依赖模块则项目内安装即可。
	
测试 gitbook 命令是否安装成功：
	
```bash
$ gitbook -V
CLI version: 2.3.2
GitBook version: 3.2.3
```

## 使用 gitbook
	
任意找一个空目录，执行：
	
```bash
$ gitbook init
warn: no summary file in this book 
info: create README.md 
info: create SUMMARY.md 
info: initialization is finished 
```
	
会在当前目录下创建出两个文件，分别是：
	
```
README.md
SUMMARY.md
```
	
暂且先不管其他的，我们现在可以直接运行试试，先把流程走通：
	
```bash
$ gitbook build
$ gitbook serve
```
	
上面的 `gitbook build` 是编译整个 `markdown` 文件，然后在当前目录生成 `_book` 目录，里面是 html 页面。这个主要在部署的时候用到。
	
而 `gitbook serve` 是本地调试开启服务命令，项目最终是要成网站的，因此, 该命令可以开启本地 `http://127.0.0.1:4000` 地址作为网站浏览地址。
	
假如大家执行 `gitbook serve` 出错，建议大家先 `gitbook build` 在 `gitbook serve`.
	


## 参考链接
1. [https://redis.io/](https://redis.io/)
2. [https://jiyiren.github.io/2018/08/04/kafka/](https://jiyiren.github.io/2018/08/04/kafka/)
3. [http://gitbook.zhangjikai.com/themes.html](http://gitbook.zhangjikai.com/themes.html)
4. [http://www.chengweiyang.cn/gitbook/](http://www.chengweiyang.cn/gitbook/)
5. [https://www.cnblogs.com/YangJieCheng/p/7991660.html](https://www.cnblogs.com/YangJieCheng/p/7991660.html)
