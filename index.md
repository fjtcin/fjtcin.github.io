---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home Page
---

> A journey of a thousand miles begins with a single step. ― [Laozi](https://en.wikipedia.org/wiki/Laozi)

[About Me]({% link about.md %})

---

Posts are listed below.

<ul>
  <li>Mathematics
    <ul>
      {% for post in site.categories.math %}
        {% if post.url %}
          {% if post.latex %}
            <li><a href="{{ post.url }}">{{ post.latex }}</a></li>
          {% else %}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
          {% endif %}
        {% endif %}
      {% endfor %}
    </ul>
  </li>
</ul>

---

[简体中文]({% link cn.md %})
{: style="text-align:center;"}
