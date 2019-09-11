---
layout: default
---
# Hackathon Hackers Europe
We're hosting a casual meet-up for UK and European hackathon organisers!

This **unconference** is a chance to meet and chat with other hackathon organisers from across the UK. 

We'll also be hosting a watch party for Hackcon Digital in the afternoon!

## Why are we running this event?
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

## Is this a Major League Hacking (MLH) event?
Technically, no. This event is split into two parts:

### **Morning** – Unconference
Independent of any event or company, Aaron, Robbie and Joe wanted to host meet-ups for UK organisers. The unconference
takes place in the morning and will consist of discussion groups and networking.

### **Afternoon** – Hackcon Digital Watch Party
We'll be hosting a watch party for [Hackcon Digital](https://hackcon.mlh.io/events/hackcon-digital/) in the afternoon.
Hackcon Digital is an MLH-run online conference.

## Why is this event free?
This unconference is an opportunity to meet up with other UK and European hackathon organisers. We'll provide food and
host casual discussion groups, and we believe this event should be as accessible as possible to hackathon organisers.

<small>Behind the scenes, this event leverages [HackNotts](https://www.hacknotts.com/)' and
[DurHack](https://durhack.com)'s resources. This event is funded separately by its own sponsors.</small>

## Do you cover travel reimbursements?
We are planning to offer travel reimbursements to participants who are coming from outside Nottingham. We're still
ironing out the details right now!

<small>Psst – don't forget your tech society or hackathon budget might be able to cover your travel!</small> 

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
