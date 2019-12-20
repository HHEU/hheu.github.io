---
layout: defaultConf
---
# Hackathon Hackers Europe
We hosted a casual meet-up for UK and European hackathon organisers!

This **unconference** was a chance to meet and chat with other hackathon organisers from across the UK. 

We also hosted the **official watch party for Hackcon Digital in Europe** in the afternoon!

## Why did we run this event?
We think the UK organiser community is a little separated right now. This year, there's no Hackcon EU taking place,
so we three community builders decided to form our own meet-ups. 

## Who's running this event?

{% for person in site.data.team %}
<div class="meet-the-team">
    <img src="{{ person.image_path }}" class="meet-the-team-image" width="150" height="150" />
    <div class="meet-the-team-text">
        <h3>{{ person.name }}</h3>
        {{ person.description | markdownify }}
    </div>
</div>
{% endfor %}

## Was this a Major League Hacking (MLH) event?
Yes and no! This event comprises two parts: 

### **Morning** – Unconference
Independent of any event or company, Aaron, Robbie and Joe wanted to host meet-ups for UK organisers. The unconference
took place in the morning and consisted of discussion groups and networking. This unconference is kindly supported
by our sponsors.

### **Afternoon** – Official Hackcon Digital Watch Party
We hosted the official MLH watch party for [Hackcon Digital](https://hackcon.mlh.io/events/hackcon-digital/) in 
Europe in the afternoon. Hackcon Digital is an MLH-run online conference and we're pleased to be the official watch
party for European hackathon organisers.

## Why is this event free?
This unconference was an opportunity to meet up with other UK and European hackathon organisers. We provided food and
host casual discussion groups, and we believe this event should be as accessible as possible to hackathon organisers.

<small>Behind the scenes, this event leverages [HackNotts](https://www.hacknotts.com/)' and
[DurHack](https://durhack.com)'s resources. This event is funded separately by its own sponsors.</small>

## Do you cover travel reimbursements?
Yes! We can offer travel reimbursements to all our attendees thanks to the generosity of our sponsors.

### If you're coming from **England**
We covered up to **£50** per person.

### If you're coming from **outside England**
We covered up to **£70** per person.

### What kind of travel will you reimburse?
We reimburseed you for any **standard class** travel by public transport that gets you to/from Nottingham.

If you drive, we payed **45p per mile**, up to the maximum amounts described above.

<small>Psst – don't forget your tech society or hackathon budget might be able to cover your travel!</small> 

{% if site.travel_reimbursement_link %}
<a href="{{ site.travel_reimbursement_link }}" target="_blank" class="btn travel-btn">Claim your travel reimbursement here</a>
{% endif %}

# Sponsors
<div class="image-container sponsors">
We were proudly supported by:
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
