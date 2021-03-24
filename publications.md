---
layout: default
---

# Publications/Presentations
## Publications
{% for item in site.data.publications %}
* **{{ item.title }}**  
	{{ item.authors }}  
	{{ item.pub-type }}  
	{{ item.date }} {% if item.award %}  
	**{{ item.award }}** {% endif %}  
	[[pdf]]({{ item.pdf }}) [[bib]]({{ item.bib }})	{% if item.note %}  
	\* {{ item.note }} {% endif %}
{% endfor %}

## Presentations
{% for item in site.data.presentations %}
{% capture title-string %} {%- if item.link -%} [{{ item.title }}]({{ item.link }}) {%- else -%} {{ item.title }} {%- endif -%} {%- if item.lectures -%}, Lectures {% for lec in item.lectures %} [[{{ lec.lecture }}]]({{ lec.link }}) {% endfor %} {%- endif -%} {% endcapture %}
* {{ item.author }}, {{ title-string }} {% if item.note %}  
	**{{ item.note }}** {% endif %}  
	{% if item.event %} {{ item.event }}, {% endif %} {{ item.address }}  
	{{ item.date }}
{% endfor %}