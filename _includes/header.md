<h1>{{ site.title | default: site.github.repository_name }}</h1>
<h2>{{ site.description | default: site.github.project_tagline }}</h2>
<h3>Saturday 5th October 2019 | 09:15 – 17:00</h3>
<h3>The Exchange, Jubilee Campus, University of Nottingham, Wollaton Road Nottingham, NG8 1BB | <a href="https://www.nottingham.ac.uk/sharedresources/documents/mapjubileecampus.pdf" target="_blank">Map</a></h3>

{% if site.ticket_link %}
    <a href="{{ site.ticket_link }}" class="btn">Get tickets now</a>
{% endif %}

<div class="social">

{% if site.data.social.facebook %}
<a href="{{ site.data.social.facebook }}">
<img src="assets/images/facebook_white.png" width="24" height="24" />
</a>
{% endif %}

{% if site.data.social.twitter %}
<a href="{{ site.data.social.twitter }}">
<img src="assets/images/twitter_white.svg" width="24" height="24" />
</a>
{% endif %}

</div>
