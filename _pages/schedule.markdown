---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-full
title: "Home"
show_sidetoc: true
subtitle: "22-28 June 2025 Baratti – TUSCANY (Italy)"
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
                      <th>{{ header   | markdownify }}</th>
                    {% endfor %}
                    </tr>
                  </thead>
                  <tbody>
                    {% for activity in site.data.schedule.activities %}
                      <tr {% if activity.class %}class="{{ activity.class }}"{% endif %}>
                        <td>{{ activity.time   | markdownify }}</td>
                        <td>{{ activity.sunday   | markdownify }}</td>
                        <td>{{ activity.monday   | markdownify }}</td>
                        <td>{{ activity.tuesday | markdownify }}</td>
                        <td>{{ activity.wednesday   | markdownify }}</td>
                        <td>{{ activity.thursday   | markdownify }}</td>
                        <td>{{ activity.friday   | markdownify }}</td>
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
        {% for speaker in site.data.speaker-cards %}
                <div class="row py-3 my-3 project" >
                        <div class="col-md-4">
                            <div class="project-img"><img src="{{site.baseurl}}{{ speaker.img_url}}" alt="{{ speaker.name }}" style="width:100%"></div>
                        </div>
                        <div class="col-md-8">
                            <div class="project-body">
                                <h5>{{ speaker.name }} </h5>
                                <p><strong> {{ speaker.institution }}</strong></p>
                                <p>{{ speaker.description }}</p>
                                {% assign topics = speaker.topics | split: "," %}
                                <p class="students">
                                <em><strong>Topic</strong>:
                                    {% for topic in topics %}
                                        {% if forloop.last %}
                                            <span>{{ topic | strip |  replace: '[', ''  |  replace: ']', '' |  replace: '"', '' }}.</span>
                                        {% else %}
                                            <span>{{ topic | strip |  replace: '[', ''  |  replace: ']', '' |  replace: '"', '' }}, </span>
                                        {% endif %}
                                    {% endfor %}
                                </em></p>
                            </div>
                        </div>
                </div>
        {% endfor %}
</div>