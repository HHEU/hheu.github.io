<h1>{{ site.title | default: site.github.repository_name }}</h1>
<h2>{{ site.description | default: site.github.project_tagline }}</h2>

{% if site.ticket_link %}
    <a href="{{ site.ticket_link }}" class="btn">Sign up now</a>
{% endif %}
