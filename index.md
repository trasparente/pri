# Categories

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for doc in category[1] %}
      <li><a href="{{ doc.url | absolute_url }}">{{ doc.title }}</a><br>{% include widgets/datetime.html datetime=doc.date replace=true %}</li>
    {% endfor %}
  </ul>
{% endfor %}