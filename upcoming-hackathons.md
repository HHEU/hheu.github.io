---
layout: default
---

# Upcoming Hackathons

<table>
    <thead>
        <th>Date</th>
        <th>Hackathon</th>
        <th>Location</th>
    </thead>
    <tbody>
        {% assign hackathons = site.data.upcoming_hackathons | sort: "start_date" %} 
        {% for hackathon in hackathons %}
        <tr>
            <td>
                <strong>{{ hackathon.start_date | date: "%-d %b %Y" }}</strong>
                to 
                <strong>{{ hackathon.end_date | date: "%-d %b %Y" }}</strong>
             </td>
            <td><a href="{{ hackathon.url }}">{{ hackathon.name }}</a></td>
            <td>{{ hackathon.university }}, {{ hackathon.country }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>
