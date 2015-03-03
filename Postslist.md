      {% assign pages_list = site.posts %}
      {% for node in pages_list %}
        {% if node.title != null %}
          {% if node.layout == "post" %}
            <a class="sidebar-nav-item{% if page.url == node.url %} active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
          {% endif %}
        {% endif %}
      {% endfor %}
