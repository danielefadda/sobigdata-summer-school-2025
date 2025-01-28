---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-full
title: "Home"
show_sidetoc: true
subtitle: "22-27 June 2025 – Baratti (Piombino) – TUSCANY (Italy)"
header_title: "From Data to Social Innovation"
---

<div class="full-width-wrapper">
    <img src="{{ site.baseurl }}/assets/images/header.svg" alt="sbd-pattern" class="full-width-image">
</div>

<div class="registration">
    <div class="container">
        <div class="row pt-2 ">
            <div class="col-md-8 offset-md-2 col-sm-12">
                <h2>Detailed Program</h2>
                <hr>
                <p>Qui ci va qualche nota importante che è bene che le persone leggano, considerando che è la pagina più usata, è una buona posizione da sfruttara</p>
                <hr>
            </div>
        </div>
    </div>

</div>

<div class="container">
        <div class="row py-3">
            <div class="col-12">
                <div class="program-table">
                <table>
                  <thead>
                    <tr>
                    {% for header in site.data.schedule.headers %}
                      <th>{{ header | markdownify }}</th>
                    {% endfor %}
                    </tr>
                  </thead>
                  <tbody>
                    {% for activity in site.data.schedule.activities %}
                      <tr {% if activity.class %}class="{{ activity.class }}"{% endif %}>
                        <td>{{ activity.time | markdownify }}</td>
                        {% if activity.sunday.content %}
                          <td rowspan="{{ activity.sunday.rowspan }}">{{ activity.sunday.content | markdownify }}</td>
                        {% elsif activity.sunday %}
                          <td>{{ activity.sunday | markdownify }}</td>
                        {% endif %}
                        {% if activity.monday.content %}
                          <td rowspan="{{ activity.monday.rowspan }}">{{ activity.monday.content | markdownify }}</td>
                        {% elsif activity.monday %}
                          <td>{{ activity.monday | markdownify }}</td>
                        {% endif %}
                        {% if activity.tuesday.content %}
                          <td rowspan="{{ activity.tuesday.rowspan }}">{{ activity.tuesday.content | markdownify }}</td>
                        {% elsif activity.tuesday %}
                          <td>{{ activity.tuesday | markdownify }}</td>
                        {% endif %}
{% if activity.wednesday.content %}
                          <td rowspan="{{ activity.wednesday.rowspan }}">{{ activity.wednesday.content | markdownify }}</td>
                        {% elsif activity.wednesday %}
                          <td>{{ activity.wednesday | markdownify }}</td>
                        {% endif %}
{% if activity.thursday.content %}
                          <td rowspan="{{ activity.thursday.rowspan }}">{{ activity.thursday.content | markdownify }}</td>
                        {% elsif activity.thursday %}
                          <td>{{ activity.thursday | markdownify }}</td>
                        {% endif %}
{% if activity.friday.content %}
                          <td rowspan="{{ activity.friday.rowspan }}">{{ activity.friday.content | markdownify }}</td>
                        {% elsif activity.friday %}
                          <td>{{ activity.friday | markdownify }}</td>
                        {% endif %}                        
                      </tr>
                    {% endfor %}
                  </tbody>
                </table>
            </div>
        </div>
    </div>
<div>

</div>
</div>

<div class="container py-3" id="projects-container">
        <h3>All the speakers</h3>   
        {% assign sorted_speakers = site.data.speaker-cards | sort: "day" %}
            {% for speaker in sorted_speakers %}
                <div class="row py-3 my-3 project" >
                        <div class="col-md-4">
                            <div class="project-img"><img src="{{site.baseurl}}{{ speaker.img_url}}" alt="{{ speaker.name }}" style="width:100%"></div>
                        </div>
                        <div class="col-md-8">
                            <div class="project-body">
                                <h5>{{ speaker.name }} </h5>
                                <p><strong> {{ speaker.institution }}</strong></p>
                                <p>{{ speaker.bio }}</p>
                                {% assign topics = speaker.topics | split: "," %}
                            </div>
                        </div>
                </div>
        {% endfor %}
</div>