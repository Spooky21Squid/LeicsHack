---
layout: page
title: LeicsHack 2022
menu_title: Home
menu_icon: house-door
---

{:.secondary}
# {{ site.event_date }}

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
                    <a href="{{ site.baseurl }}{% link registration.md %}" class="btn">Register your interest now</a>
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

You can sign up to the hack as a lone-wolf, or join us in groups of **up to 4 people.**

## About the Hack

### Where is it
LeicsHack will be hosted **in-person** in the university's state-of-the-art informatics suite located on the top floor of the new Percy Gee building on campus. You will have the option to log in as a guest and use our Linux machines equipped with tools and development environments, or bring your own laptop.

### Covid Precautions
LeicsHack will take place in-person, so Covid precautions will be in place that everyone will have to follow like wearing masks
and social distancing where possible. To enter, **Everyone will need proof of vaccination, or proof of a negative lateral flow test taken within 24 hours of the hack.** Finalised Covid guidelines will be published closer to the event.

**Note:** Given the recent [Living with Covid-19 guidance by the government](https://www.gov.uk/government/publications/covid-19-response-living-with-covid-19), this might be subject to change. If it does, we will update our requirements.

### Food / Sleeping Arrangements
Meals will be provided throughout the event including a midnight pizza snack, and there are water fountains in the building to use to fill up
water bottles, but feel free to bring your own snacks!. There will also be a designated area for eating / drinking. After a long days coding, there
will be areas to sleep and take a break.

### Events / Games
We will run workshops throughout the hack on technical subjects to help you with your projects. Sponsors will run talks
about opportunities for students within their organisations, and run workshops about their products like APIs. Also, we are hoping
to run some minigames throughout the hack that will offer mini-prizes!

<!-- kanye-zone tournament, rubiks cube, sql-injection? -->

[FAQs]({{ site.baseurl }}{% link faq.md %})

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