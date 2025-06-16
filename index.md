index.md---
layout: splash
title: "通向世界的钥匙——6丝频道"
permalink: /
header:
  overlay_image: /assets/images/banner.jpg
  overlay_filter: 0.3
  caption: "探索世界，点亮生活"
---

<div style="display:flex;align-items:center;gap:24px;margin-top:-80px;margin-bottom:32px;">
  <img src="/assets/images/avatar.jpg" style="width:120px;height:120px;border-radius:50%;border:4px solid #fff;box-shadow:0 2px 8px rgba(0,0,0,0.1);">
  <div>
    <h2 style="margin-bottom:8px;">6丝（Yao1868）</h2>
    <div style="margin-bottom:8px;">
      大家好，我是6丝。<br>
      这里，是一扇通往世界与生活的奇妙之门。<br>
      我热爱用专业的视角和探索的好奇心，解读生活中的“小谜题”，也乐于挖掘那些意想不到的科学妙招。<br>
      无论是全球各地的新鲜趣闻，还是前沿科技和时政风向，我都愿与你一同发现、分析、分享。<br>
      在这里，你会感受到知识的乐趣、世界的神秘、生活的巧思。<br>
      让我们一起以新鲜的眼光，探索多彩的世界，把握时代脉搏，享受每一个灵感闪现的时刻！
    </div>
    <a href="https://github.com/Yao1868" style="margin-right:12px;" target="_blank">GitHub</a>
    <a href="mailto:Yao139229@gmail.com" target="_blank">邮箱</a>
  </div>
</div>

## 精选推荐
{% for post in site.categories.精选 limit:3 %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}

## 生活探秘
{% for post in site.categories.生活探秘 limit:3 %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}

## 世界风向
{% for post in site.categories.世界风向 limit:3 %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}

## 科普妙招
{% for post in site.categories.科普妙招 limit:3 %}
- [{{ post.title }}]({{ post.url }}) <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}

## 热门标签
<ul>
{% assign sorted_tags = site.tags | sort: 'last' | reverse %}
{% for tag in sorted_tags limit:10 %}
  <li><a href="{{ site.baseurl }}/tags/{{ tag[0] }}/">{{ tag[0] }}</a> ({{ tag[1].size }})</li>
{% endfor %}
</ul>