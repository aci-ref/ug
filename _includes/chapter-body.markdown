
{% capture chapter %}{{ page.path | split: '/' | first }}{% endcapture %}
{% for section in page.sections %}
{% capture filename %}{{chapter}}/{{section.name}}.markdown{% endcapture %}
## {{ forloop.index }}. {{ section.title }}     {#{{section.name}}}
{% include {{filename}} %}
{% endfor %}
