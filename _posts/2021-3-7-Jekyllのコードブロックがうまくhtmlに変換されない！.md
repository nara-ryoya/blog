---
layout: post
title:  "Jekyllのコードブロックがうまくhtmlに変換されない！"
date:   2021-03-07 00:10
# categories: jekyll update
---


前回に引き続きJekyllの話題。
markdownで以下のようにコードブロックを書くと、どうもうまくhtmlに変換されない。色々見てみると、markdownコンバーターがコードブロックのコードを実際のLiquidのコードだと勝手に解釈してしまっているようだった。

````
```
{% raw %}
{% include header.html %}
{% endraw %}
```
````

markdownのプレビューでは問題なく表示されているのに。。。
<br><br>

# 解決法 

[この記事](https://www.xmisao.com/2014/06/30/how-to-escape-liquid-tag-in-jekyll.html)で一発解決！。

