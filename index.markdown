---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
{% for post in site.pages %}
  <li><b><a href="{{ post.url }}">{{post.title}}</a></b></li>
{% endfor %}

{% for file in site.static_files %}
  {% if file.image %}
    <img src="{{file.path}}" alt="{file.name}">
  {% endif %}
  {{ file.name}}
{% endfor %}
