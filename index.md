---
layout: default
---
# Hackathon Hackers Europe 
Hackathon Hackers Europe (or HHEU for short) is an organisation targetting at helping student lead hackathons around europe. We are here to bring the hackatoh organiser and attendee community together to make hackathons easier to run and partipate in.

HHEU put on events throughout the year to help meet our objectives like the <a href="/HHEUConf.html">HHEU conference</a>.



## FAQ
{% for questions in site.data.FAQ %}
<div class="meet-the-team">
    <div class="meet-the-team-text">
        <h3>{{ questions.question }}</h3>
        {{ questions.answer | markdownify }}
    </div>
</div>
{% endfor %}

## The Team
{% for person in site.data.team %}
<div class="meet-the-team">
    <img src="{{ person.image_path }}" class="meet-the-team-image" width="150" height="150" />
    <div class="meet-the-team-text">
        <h3>{{ person.name }}</h3>
        {{ person.description | markdownify }}
    </div>
</div>
{% endfor %}

# Sponsors
<div class="image-container sponsors">
We are proudly supported by:
<div class="flagship-sponsors">
{% assign sponsors = site.data.sponsors | where:"type","sponsor" %}
{% for sponsor in sponsors %}
{% include sponsor_block.html entity=sponsor %}
{% endfor %}
</div>

<small>And powered by:</small>
<div class="image-container partners">
{% assign partners = site.data.sponsors | where:"type","partner" %}
{% for partner in partners %}
{% include sponsor_block.html entity=partner %}
{% endfor %}
</div>
</div>

# Contact
Got another question? Reach out to us on [hello@hackathonhackers.eu](mailto:hello@hackathonhackers.eu)!
