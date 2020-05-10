> 读书使人充实，讨论使人机智，笔记使人准确，
>
> 读史使人明智，读诗使人灵秀，数学使人周密，
>
> 科学使人深刻，伦理使人庄重，逻辑使人善辩。
>
> 凡有所学，皆成性格。  —— 培根

## 公式渲染  

本项目使用 [MathJax](https://www.mathjax.org) 语法书写公式，出于以下五点的考虑，最终选择本地渲染的方式来载入公式，如果要正确显示公式需要使用 [Google Chrome](https://www.google.com/chrome/) 浏览器并且安装 [MathJax Plugin for Github](https://chrome.google.com/webstore/detail/mathjax-plugin-for-github/ioemnmodlmafdkllaclgeombjnmnbima/related) 插件
- 方便后期导出 PDF 格式文档
- 第三方 API 渲染效果不如本地渲染且无法居中对齐
- 使用第三方 API 可能存在某天网站服务停止的情况
- 维护成本较低，内容简介明了，要修改的细节可以快速修改
- 在离线阅览的情况下，Markdown 编辑器可以正常显示公式

## 物理  
[	第一章：运动的描述 匀变速直线运动](物理/第一章：运动的描述%20匀变速直线运动.md)  
[第二章：相互作用]()  
[第三章：牛顿运动定律]()  
[第四章：曲线运动 万有引力与航天](物理/第四章：曲线运动%20万有引力与航天.md)  
[第五章：机械能]()  
[第六章：动量]()  
[第七章：静电场]()  
[第八章：恒定电流](物理/第八章：恒定电流.md)  
[第九章：磁场]()  
[第十章：电磁感应](物理/第十章：电磁感应.md)  
[第十一章：交变电流 传感器]()  
[第十二章：近代物理初步](物理/第十二章：近代物理初步.md)  
[第十三章：热学]()  
[第十四章：波与相对论](物理/第十四章：波与相对论.md)  

## 化学  
[专题一：化学家眼中的物质世界]()  
[专题二：离子反应与氧化还原反应]()  
[专题三：金属及其化合物]()  
[专题四：非金属及其化合物]()  
[专题五：微观结构与物质的多样性]()  
[专题六：化学反应与能量转化]()  
[专题七：化学反应速率和化学平衡]()  
[专题八：水溶液紫红的离子反应]()  
[专题九：有机物的获取与应用]()  
[专题十：有机化学基础]()  
[专题十一：物质结构与性质]()  
[专题十二：化学实验]()  

## 文件命名规范  
- 不能包含：< > / \ | :  * ?   
- 文件名中的冒号使用中文冒号  
  
## 内容编辑规范  
- 中文与字母或者数字之间前后要用空格  
- 使用 [Markdown TOC generate](https://magnetikonline.github.io/markdown-toc-generate/) 生成 TOC 目录
- 文本换行：GitHub 文章换行需要在行尾加上两个空格实现，编辑完 Markdown 文本后使用下面这条命令自动补全行尾  
```  
sed -i '' -e 's/  $//' -e 's/$/  /' README.md  
```
- 加空白行：
  
  ```
  &nbsp;
  ```
  
  
  
- 更多规范请参考 [中文文案排版指北（简体中文版）](https://github.com/mzlogin/chinese-copywriting-guidelines)
## 图片编辑规范 

- 直线图：[SVG](http://www.w3.org/Graphics/SVG/)&ensp;[使用教程](https://www.runoob.com/svg/svg-tutorial.html)

- 流程图：[Graphviz](https://www.graphviz.org)&ensp;[使用文档](https://graphviz.gitlab.io/documentation/)
- 函数图：[Matplotlib](https://github.com/matplotlib/matplotlib) &ensp;[使用文档](https://matplotlib.org/users/pyplot_tutorial.html)
- 结构式：[Overleaf](https://www.overleaf.com) + [chemfig](https://www.ctan.org/pkg/chemfig)&ensp;[使用教程](https://www.overleaf.com/learn/latex/chemistry_formulae)
- 电路图：[Overleaf](https://www.overleaf.com) + [CircuiTikz](https://github.com/circuitikz/circuitikz) &ensp;[使用教程](https://www.overleaf.com/learn/latex/CircuiTikz_package)
- 图片原始文件必须为可编辑类型，有原始文件并保存在学科目录的 media 文件夹下。例如 svg、tex
- 引用图片下方应有序号标注并与图片文件名相同。例如 Fig 1. 电子跃迁  
  
## Markdown 编辑器  
推荐使用免费好用且兼容 Windows、macOS 和 Linux 的 [Typora](https://typora.io)  
下载后需要在设置中开启 Markdown 语法扩展下的所有选项  

## Todo  
- [ ] 自动化 TOC
- [ ] Travis-CI + matplotlib + makefile  
- [ ] 后期内容基本编辑完成后在提供图片格式支持
