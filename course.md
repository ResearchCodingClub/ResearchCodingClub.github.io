---
layout: page
title: Research Coding Course
subtitle: Skills and training for people developing research software
---

Over the years we have developed extensive training materials and delivered
hands-on tutorials and seminars to hundreds of researchers on everything from
testing your code to how CPUs work. This year, we're building on the University
of Sheffield's excellent [FAIR²4RS][fair24rs] course to deliver a training
programme that will teach you a whole range of skills.

## Outline of the Programme

<!-- Maintainers: Add session info in _data/course_sessions.yml -->

<span style="color: #ff0000">Dates in red are to be confirmed</span>:

{% for session in site.data.course_sessions %}
- **[{{ session.title }}](#{{ session.title | slugify }})**,
  {% if session.confirmed -%}*{{ session.date }}*{% else %}<span style="color: #ff0000">*{{ session.date }}*</span>{%- endif -%},
  {% if session.sign_up_form -%}[**sign up here!**]({{ session.sign_up_form }})
  {%- else -%}<span style="color: #ff0000">Sign-up form coming soon!</span>
  {%- endif -%}
{%- if session.repeat %}
  - Repeated {% if session.repeat.confirmed -%}*{{ session.repeat.date }}*{% else %}<span style="color: #ff0000">*{{ session.repeat.date }}*</span>{%- endif -%},
    {% if session.repeat.sign_up_form -%}[**sign up here!**]({{ session.repeat.sign_up_form }})
    {%- else -%}<span style="color: #ff0000">Sign-up form coming soon!</span>
    {% endif %}
{%- endif -%}
{% endfor -%}

<br>

### Target Audience and Prerequisites
We welcome everyone working with research software, from undergraduates to
professors, from beginners to experts, and from people who create analysis
scripts on their laptops to those who run first principles modelling on
supercomputers.

Each session will have some individual prerequisites. Some experience with
developing research software or scripts, for example in Python or R, might be
needed. Please refer to the individual course details to know what they are.

## FAQs

#### Why are hands-on and tutorial sessions in-person only?

We are all volunteers, and we don't have dedicated resources for creating and
delivering this course, and unfortunately, we have found that it takes a lot
more effort to effectively deliver hands-on material online -- and even more to
deliver hybrid sessions.

#### I missed a session, will you repeat it?

We repeat our most popular sessions, particularly Introduction to Version
Control a couple of times a year, and we record all our online sessions and make
the recordings available. All our slides and other material are also available.

You can see our previous courses, sessions, and activities in our [archive](/archive).

#### Do I need to bring my own computer to hands-on sessions?

We run our all hands-on sessions in a PC room on campus, so you can use either
Windows or Linux on the dual-boot PCs, or bring your own laptop.

{% for session in site.data.course_sessions %}
### {{ session.title }}
- {% if session.confirmed -%}**{{ session.date }}**{% else %}<span style="color: #ff0000">{{ session.date }}</span>{%- endif -%}
  {%- if session.sign_up_form %}
  - [**Sign up here!**]({{ session.sign_up_form }})
  {%- else %}
  - <span style="color: #ff0000">Sign-up form coming soon!</span>
  {%- endif %}
  - {% if session.online %}Online{% else %}In person{% endif %}
{%- if session.repeat %}
- {% if session.repeat.confirmed -%}**{{ session.repeat.date }}**{% else %}<span style="color: #ff0000">{{ session.repeat.date }}</span>{%- endif -%}
  {%- if session.repeat.sign_up_form %}
    - [**Sign up here!**]({{ session.repeat.sign_up_form }})
  {%- else %}
    - <span style="color: #ff0000">Sign-up form coming soon!</span>
  {%- endif %}
  - {% if session.repeat.online %}Online{% else %}In person{% endif %}
{%- endif %}

{{ session.synopsis }}

{% endfor %}

## Learning outcomes
After completing this modular programme, participants should be able to:

- Understand the FAIR principles and describe how they apply to research software
- Explain how applying FAIR principles to research software can support open research goals such as transparency, reproducibility and reusability
- Identify actions that can be taken at different stages of the research lifecycle to enhance the FAIRness of their research software outputs
- Develop a plan addressing the intended scope, impact and lifespan of their research software
- Describe different types of software licence and discuss their potential implications for reuse of research software, including commercialisation
- Apply best practices for scientific software development including design, version control, testing, continuous integration and documentation
- Associate their research software with a unique and persistent identifier and use metadata to enhance its findability, accessibility and reusability
- Identify repositories that provide long-term persistent storage for research software
- Apply approaches such as packaging and containers to enhance the reusability and reproducibility of research software.

# Feedback

We'd love to hear your (anonymous) feedback: please fill in our [feedback form][feedbackform].

[fair]: https://doi.org/10.1038/sdata.2016.18
[fair24rs]: https://rse.sheffield.ac.uk/training/fair4rs/
[session1form]: https://forms.gle/GMYnMMGUuf58JkE48
[session2form]: https://forms.gle/38267pioXj8qd9ie6
[session3form]: https://forms.gle/HPSACtgKzRU2XM6r8
[feedbackform]: https://forms.gle/t4oJMCPi8wuzJtik7
[session4form]: https://forms.gle/fC2XVFSxfcb2KsyQ9
[session5form]: https://forms.gle/8tbkbNXyhwasnhGg7
[session6form]: https://forms.gle/3ohpUuCEasVLcPB77
[session7form]: https://www.eventbrite.co.uk/e/university-of-york-research-coding-club-publishing-your-software-in-joss-tickets-1984310025703
[session8form]: https://forms.gle/cnz2FL91bP3tWGjX8
[session9form]: https://forms.gle/VAZhdxqZDaMhsMqD6

[intro_slides]: https://docs.google.com/presentation/d/1P5dHCa6yvODlx7i6l89083gR-PpTCYsTQI1QgcqGS2k
[intro_video]: https://york-ac-uk.zoom.us/rec/share/RNQpldj13NL53AoEl0F0Y2OyVHImt0m_hmLHVZVSXOqq4XwNUd9mc8eWLWkbLHnz.HQpZ8VwJWr11mr17

[git_slides]: https://docs.google.com/presentation/d/1ifKyvCnR-ZcJokvKrrfUbf9n7lmIrP8XKRz9Uqyu538

[lifecycle_slides]: https://docs.google.com/presentation/d/1pAwfg1H5Ny957NRrUlNhCRizVs4AkuBooYWcL7zu6i0
[lifecycle_video]: https://york-ac-uk.zoom.us/rec/share/TEg2AYluX9azyfP7N7hHQyR8OpMJStxWS8Unpv8syIcK43wujSI0212PupSoVN0x.uMEyU-9ZBsIXKEEc

[testing_lesson]: https://researchcodingclub.github.io/python-testing-for-research
[testing_files]: https://github.com/ResearchCodingClub/python-testing-for-research/tree/main/learners/files

[rep_env_slides]: https://docs.google.com/presentation/d/144TqQoYIj1OgbIpQ4JDZmLnx4FtMsg3WL7cvf6N914A/edit?usp=sharing
[rep_env_video]: https://york-ac-uk.zoom.us/rec/share/tbZdpdrLcr1JXg-bYcLTB7EHXe8gurgkw1VDL0mAOnCSez61DLKJhMlWYro73H5V.0QibsuCK4VIvDNVZ

[docs_lesson]: https://researchcodingclub.github.io/documentation/

[joss_slides]: https://researchcodingclub.github.io/slides/2026-04-15-publishing-in-joss.pdf
[joss_video]: https://york-ac-uk.zoom.us/rec/share/KQsK3YR4RGTitZrsuGJMXhCIqzd1GeGcjsmMtXOFtEO7nkEcRXBFVEcX7WkDjeia.Bzf74IFgSmsw_W2I

[packaging_slides]: /slides/2026-05-06-packaging.pdf
[R_packaging]: https://3mmarand.github.io/make-an-r-pkg/minimal-package.html
