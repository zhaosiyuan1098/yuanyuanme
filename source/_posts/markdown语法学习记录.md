---
title: markdown语法学习记录
date: 2022-11-28 20:32:36
tags: markdown
katex: true
categories:
- 学习
---
# markdown语法学习
学习下markdown基本语法，方便记笔记。
## 参考
[视频](https://www.bilibili.com/video/BV1JA411h7Gw/?spm_id_from=333.337.search-card.all.click&vd_source=e7ba1b5c6c81d48eeecd2099401b1614"b站链接")


[官方教程](https://markdown.com.cn/)

## 测试

### 已实现
引用：

>这是一段引用

排序：

放冰箱:

1. 开
2. 关
3. 哈哈哈

打勾的表：

明天:
- [x] 吃饭
- [ ] 睡觉

代码块：
```c++

int main(){
    std::cout<<"hello!markdown!";
}

```

数学公式： 
$$2\sqrt{a}x$$

表格：
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

------
分割线


插入链接：

[百度](baidu.com"一个搜索引擎”)


插入图片：

 ![baidu](../images/tuanzi.png)


字体：

 *斜体*

 **加粗**

 `行间代码`

  :smile:

  $\theta=x^2$

  ---

  ### 嵌入视频测试

<iframe src="//player.bilibili.com/player.html?aid=327623069&bvid=BV1JA411h7Gw&cid=171385214&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

  ---

  ### 高亮测试

  ==hightlight test==

  不知道为啥亮不了，哥们写的是` ==hightlight test== `

  ### 脚注测试

  Here's a sentence with a footnote. [^1]
    
    [^1]: This is the footnote.

----
## 踩坑

本人使用hexo-themo-yun完成搭建，在测试时出现了*latex*公式无法正常显示的问题，但实际上该主题的[官方文档](https://yun.yunyoujun.cn/guide/additional-package-support.html)已经给出了katex解决办法，在hexo的`_config.json`文件末端写入
```
katex:
  copy_tex: true
  global: false
  options: {}
```
后，在需要使用的katex的markdown文档中，仅需在开头处指定katex为true，并注意下一行写下公式即可实现公式显示，切勿轻易尝试卸载hexo-math。




