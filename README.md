![image](https://github.com/user-attachments/assets/32161099-693f-49e6-8e29-edff5ed6061a)# use_elsevier_latex_experience
使用elsevier期刊latex模板的经验

首先下载elsarticle模板，下载地址：https://www.elsevier.com/researcher/author/policies-and-guidelines/latex-instructions

elsarticle.cls已默认加载宏包：
natbib.sty用于管理参考文件，设置参考文献的显示方式
geometry.sty用于设置页边距
grapgicx.sty用于插入图片
hyperref.sty用于设置超链接
pifont.sty和txfonts.sty用于设置数学公式和正文字体
fleqn.clo用于设置方程公式的对齐方式

\documentclass[<options>]{elsarticle}
  preprint 默认选项，单倍行距
  review 双倍行距 (推荐，方便审稿人审稿)
  1p(3p,5p)1p,页芯 13.5cmx19.75cm,单栏;
            3p,页芯 16.45cmx21.9cm,可设置双栏(twocolumn)
            5p,页芯 18.35cmx24cm,双栏
  authoryear 传给 natbib.sty,参考文献使用作者年形式
  number 传给 natbib.sty,参考文献按引用顺序排版
  sort&compress 配合 number 选项,排序并压缩, 如 [1-5]
  longtitle 标题摘要等 frontmatter 内容太长,使用此选项分割
  times 使用 Times New Roman 字体

  
article.cls的其他选项，默认开启a4paper,10pt,oneside,onecolumn,preprint
参考文献格式的设置：
\biboptions{longnamesfirst,angel,semicolon}
超链接设置：\hypersetup{}
页边距设置：\geometry{}

投稿期刊:\journal{期刊名称}
标题,作者信息,摘要,关键词等内容放入 frontmatter 环境中

标题及标题脚注

\title{This is a specimen title\tnoteref{t1,t2}}
\tnotetext[t1]{This document is a collaborative effort.} ##设置自助信息
\tnotetext[t2]{The second title footnote...}

![image](https://github.com/user-attachments/assets/c7d47ece-769f-465c-bdc2-a1f8eb991d03)






