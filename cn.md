---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: 主页
---

[我的知乎](https://www.zhihu.com/people/fjtcin)

[陈发来线代听课笔记]({% link cn/linear-algebra-and-analytic-geometry.md %})

[柏拉图《申辩篇》读书笔记]({% link cn/plato.md %})

---

Posts are listed below.

<ul>
  <li>英语学习
    <ul>
      <li>纪录片：空中浩劫
        <ul>
          {% for post in site.categories.mayday %}
            {% if post.url %}
              <li><a href="{{ post.url }}">{{ post.title }}</a></li>
            {% endif %}
          {% endfor %}
        </ul>
      </li>
    </ul>
  </li>
</ul>

---

[English]({% link index.md %})
{: style="text-align:center;"}
