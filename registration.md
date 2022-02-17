---
title: LeicsHack registration
menu_title: Registration
menu_icon: clipboard-check
event_status:
 - soon
---

{:.lead}
**Any student from any university** is encouraged to take part, especially 1st years and students that haven't been to a hackathon
before. {% if site.registration_status
== "soon" or site.registration_status == "demo" %}Registration opens on
{{ site.registration_opens_date }}.{% endif %} The closing date for applications
is {{ site.registration_closes_date }}.

<div class="aside" markdown="1">
Join us at LeicsHack on {{ site.event_date }}!.

{% if site.registration_status == "soon" or site.registration_status == "demo" %}
  [Register your interest now](https://bit.ly/3gFpH6Z){:.btn target="_blank"}
{% endif %}
{% if site.registration_status == "open" or site.registration_status == "demo" %}
  [Complete the application form](https://bit.ly/3gFpH6Z){:.btn target="_blank"}
{% endif %}
{% if site.registration_status == "closed" or site.registration_status == "demo" %}
  <a class="btn disabled">Registration has closed</a>
{% endif %}

The closing date for applications is {{ site.registration_closes_date }}.
</div>

<!--
We are looking for enthusiastic and dedicated researchers who already have
experience with analysing ... data, and who are keen to experience working with
different scientists and institutes, and perhaps on topics not immediately in
their area. We also intend that early career researchers[<sup>(?)</sup>][faq]{:title="What do we mean by an Early Career Researcher (ECR)?"},
will build strong relationships with their peers from other institutes. 

This virtual event will require approximately two hours commitment prior to the
hackathon, and then X days commitment during the event, which will take part
from **{{ site.event_date }}**. Technical support and guidance will be provided
by the [Jean Golding Institute](https://www.bristol.ac.uk/golding/) at the
University of Bristol, but we expect all applicants to have prior knowledge of
scientific programming.

We will supply each researcher with a temporary hackathon account on ..., which
will give then access to a Python&nbsp;3 notebook environment and a variety of
relevant datasets, for which we can provide technical support and guidance.
Researchers may be able to use other programming languages and tools, however we
will only be able to provide limited support for these.

If you are interested in applying and having the opportunity to engage with
like-minded scientists, then please complete the application form by clicking
the link above. Please be aware that this event will only be open to those
residing in UK academic institutions.
-->

Registration will open on {{ site.registration_opens_date }}, but for now, **register your interest** and be emailed when
registration goes live! The closing date for the applications is {{ site.registration_closes_date }}. If
you have any queries, or have any difficulties completing the registration form, please email: <{{ site.mailbox_address }}>.

[faq]: {{ site.baseurl }}{% link faq.md %}
