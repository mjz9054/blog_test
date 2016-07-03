---
layout: default
title: GitHub Pages 代码高亮
---

---

### 支持Markdown语法的代码高亮

例如：

```java
   public static void main(String[] args){
        System.out.println("Hello GitHub Pages");
   }
```

### 1.配置_config.yml

    markdown: redcarpet
    redcarpet:
        extensions: ["fenced_code_blocks", "autolink", "tables", "strikethrough"]


### 2.引入语法高亮的css文件

    <link href="{{ site.baseurl }}/css/syntax.css" rel="stylesheet" type="text/css">

---

*注：通过修改css文件，应用不同的高亮配色方案*


