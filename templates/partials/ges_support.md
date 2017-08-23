
### Support
<hr>

<ul class="fa-ul">

<li><i class="fa-li fa fa-life-ring fa-lg"></i>

Contact pour le réseau de la santé québécois:

</li>
</ul>

<!-- Look the author details up from the site config. -->
{% set author = config.authors.authors['françoise'] %}
<!-- Output author details if some exist. -->
{% if author.mug %}
<!-- Photo author -->
<img src="{{ page.find('/images/authors').media[ author.mug ].url }}" class="author"  alt="Une photo de {{ author.name }}" />
<span itemprop="author" itemscope itemtype="http://schema.org/Person"><span itemprop="name" class="pr20 icon-edit"><a href="mailto:{{ author.email | safe_email }}" target="_blank"> {{ author.name }}</a></span>
</span>
{% elseif author.email %}
<!-- Gravatar -->
<img src="{{ author.gravatar }}" class="author" alt="Une photo de {{ author.name }}" />
<span itemprop="author" itemscope itemtype="http://schema.org/Person"><span itemprop="name" class="pr20 icon-edit"><a href="mailto:{{ author.email | safe_email }}" target="_blank"> {{ author.name }}</a></span>
</span>
{% endif %}
