{% for coll in site.collections %}
  {{ coll|inspect }}
{% endfor %}

{% for cat in site.categories %}
### {{ cat[0] }}
{% for item in cat %}
-  {{ item|inspect }}
{% endfor %}
{% endfor %}