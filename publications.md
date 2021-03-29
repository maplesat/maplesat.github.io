---
layout: default
---

# Publications/Presentations
## Publications
{% for item in site.data.publications %}
{% capture links %}
{%- if item.pdf -%} [[pdf]]({{ item.pdf }}) {% endif %}
{%- if item.bib -%} [[bib]]({{ item.bib }}) {% endif %}
{%- if item.slides -%} [[slides]]({{ item.slides }}) {% endif %}
{%- if item.talk -%} [[talk]]({{ item.talk }}) {% endif %}
{% endcapture %}

* **{{ item.title }}**  
	{{ item.authors }} {% if item.pub-type %}  
	{{ item.pub-type }} {% endif %} {% if item.date %}  
	{{ item.date }} {% endif %} {% if item.award %}  
	**{{ item.award }}** {% endif %}  
	{{ links }}	{% if item.note %}  
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