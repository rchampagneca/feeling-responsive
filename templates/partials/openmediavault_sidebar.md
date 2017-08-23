### Tous les guides d'installation

{% set q = page.collection({'items':{'@taxonomy':{'category': 'OpenMediaVault'}},'order': {'by': 'default', 'dir': 'asc'}}) %}
<ul class="side-nav">
{% for p in q %}
<li><a href="{{  p.url }}"><strong>{{ p.title }}</strong></a></li>
{% endfor %}
</ul>
