---
layout: page
title: LeicsHack 2022
menu_title: Home
menu_icon: house-door
---

{:.secondary}
# {{ site.event_date }}

{:.lead}
**Hey, welcome to LeicsHack!** The idea for LeicsHack was only conceived very very recently and as such, the website is
still being updated.

<div class="aside">
    <h2><i class="bi bi-calendar3"></i> Event timeline</h2>
    <dl>
        {% if site.registration_status == "soon" or site.registration_status == "open" or site.registration_status == "demo" %}
            <dt>{{ site.registration_opens_date }}</dt>
            <dd>
                Applications open for participants<br>
                {% if site.registration_status == 'open' %}
                    <a href="{{ site.baseurl }}{% link registration.md %}" class="btn">Register now</a>
                {% elsif site.registration_status == 'closed' %}
                    <a class="btn disabled">Registration has closed</a>
                {% elsif site.registration_status == 'soon' %}
                    <a class="btn disabled">Registration opens soon</a>
                {% endif %}
            </dd>
        {% endif %}

        <dt>{{ site.registration_closes_date }}</dt>
        <dd>Applications close</dd>

        <dt>{{ site.event_date }}</dt>
        <dd>Hackathon date</dd>
    </dl>
</div>

{% if site.event_status != "over" %}

Hey, we're LeicsHack (pronounced Let's Hack) 2022! For the first time in a very long time, a hackathon has come to Leicester.
LeicsHack will last 24 hours on {{ site.event_date }} starting at 12pm, and is organised for students, by students.

**Any student from any university** is encouraged to take part, especially 1st years and students that haven't been to a hackathon
before. It would be nice if the LeicsHack team wasn't the only new face entering the hackathon scene!

## LeicsHack is In-person

LeicsHack will take place in-person, (hopefully) on the University of Leicester's campus. Food will be provided throughout the
event, as well as areas to sleep after a long day of coding. We will have mini-events running too like games (Kanye-zone tournament anyone?), talks from sponsors, and workshops. Covid precautions will be in place that everyone will have to follow like wearing masks
and social distancing where possible. More details will be announced closer to the hack!

[faq]: {{ site.baseurl }}{% link faq.md %}

{% else %}

Scientists from the University of Bristol hosted a X-day hackathon on
{{ site.event_date }}, open to researchers, to...

Researchers could sign up to [topics ranging from]({{ site.baseurl }}{% link projects.md %})
... to ..., and more. Teams were be led by senior academics from a range of
disciplines at the University of Bristol, but participating researchers could be
from any UK academic institution.

The event took place virtually, using a combination of **video conferencing**
(Zoom) for meetings and seminars, and **discussion forums** (Slack) for ongoing
comms. Data holding and analysis took place on...

{% endif %}