---
layout: page
title: "Tags"
description: "文章印象"  
header-img: "img/semantic.jpg"  
---

## 本页使用方法

1. 在下面选一个你喜欢的词
2. 点击它
3. 相关的文章会「唰」地跳到页面顶端
4. 马上试试？

***
## 印象列表


<div id="tagcloud">
{% for tag in site.tags %}
<a href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="{{ tag[1].size }}" style="color:#12b5ad">{{ tag[0] }}</a>
{% endfor %}
</div>

***

<ul class="listing">
{% for tag in site.tags %}
  <h2 class="listing-seperator" id="{{ tag[0] }}" >{{ tag[0] }}</h2>
{% for post in tag[1] %}
  <li class="listing-item">
  <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
  <span>&nbsp;&nbsp;</span>
  <a href="{{ post.url }}" title="{{ post.title }}" style="color:blue">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>


<script src="/js/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script> 
<script language="javascript">
$.fn.tagcloud.defaults = {
  size: {start: 14, end: 18, unit: 'pt'},
  color: {start: '#cde', end: '#f52'}
};

$(function () {
  $('#tagcloud a').tagcloud();
});
</script>

