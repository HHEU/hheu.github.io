<h1>{{ site.title | default: site.github.repository_name }}</h1>
<h2>{{ site.description | default: site.github.project_tagline }}</h2>
<h3>Saturday 5th October 2019 | Nottingham, UK</h3>

{% if site.ticket_link %}
    <a href="{{ site.ticket_link }}" class="btn">Get tickets now</a>
{% endif %}
