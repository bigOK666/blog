---
title: "更改博客字体"
date: 2023-06-15T22:59:29+02:00
draft: false
---

## 选择字体

受[莉莉](https://lillianwho.com/)博客字体的启发，找到了**霞鹜文楷 LXGW WenKai**这个超喜欢的字体，最后选择了其变体 LXGWBright，是中英文合并的字体，下载 ttf: https://github.com/lxgw/LxgwBright/releases

## 为站点添加字体

在主站的根目录下，找到或者创建`static`文件夹，在这个文件夹下继续创建`fonts`文件夹，然后将下载的字体文件(LXGWBright-Regular.ttf)拷贝到`fonts`文件夹下。

## 启用字体

在主站的根目录下，找到或者创建`assets`文件夹，在这个文件夹下继续创建`css`文件夹，然后创建文件`custom.css`。在这个 css 文件中添加如下内容：

```
@font-face {
    font-family: lxgwbright-regular;
    src: url('/fonts/LXGWBright-Regular.ttf');
}

html {
    font-family: lxgwbright-regular;
    font-size: 14pt;
}
```

`@font-face`是用来定义字体变量的，全站使用字体和字号只需要在`html`中更改字体和字号。

搞定！
