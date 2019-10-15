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
        {% for hackathon in site.data.upcoming_hackathons %}
        <tr>
            <td>{{ hackathon.start_date }} to {{ hackathon.end_date }}</td>
            <td><a href="{{ hackathon.url }}">{{ hackathon.name }}</a></td>
            <td>{{ hackathon.university }}, {{ hackathon.country }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>
