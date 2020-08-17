---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home #default

# You can link individual posts like this...
#[post](../test/2020/08/13/test-post-1.html)
#[post](../test/2020/08/13/test-post.html)

---

<!---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

-->

<!---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br>{{ post.date }}
      <br>{{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

-->

<!---

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

-->

<!---
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

-->

<!---

<ul>
{% for category in site.categories %}
  {% assign category_name = category[0] %}
  <li>
    <a href="/category/{{ category_name | slugify }}/">{{ category_name | replace: "-", " " }}</a>
  </li>
{% endfor %}

-->