---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-full
title: "Home"
show_sidetoc: true
subtitle: "22-28 June 2025 – Baratti (Piombino) – TUSCANY (Italy)"
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
                <p class="lead">
                    The school is organized in two parts: in the morning students will attend lectures with different speakers, while in the afternoon they will work on group projects guided by dedicated tutors.
                </p>
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
          <td rowspan="{{ activity.sunday.rowspan }}"><i class='fas fa-{{ activity.sunday.content.icon }}'></i> {{ activity.sunday.content.text | markdownify }}</td>
        {% elsif activity.sunday %}
          <td><i class='fas fa-{{ activity.sunday.icon }}'></i> {{ activity.sunday.text | markdownify }}</td>
        {% endif %}
        {% if activity.monday.content %}
          <td rowspan="{{ activity.monday.rowspan }}"><i class='fas fa-{{ activity.monday.content.icon }}'></i> {{ activity.monday.content.text | markdownify }}</td>
        {% elsif activity.monday %}
          <td><i class='fas fa-{{ activity.monday.icon }}'></i> {{ activity.monday.text | markdownify }}</td>
        {% endif %}
        {% if activity.tuesday.content %}
          <td rowspan="{{ activity.tuesday.rowspan }}"><i class='fas fa-{{ activity.tuesday.content.icon }}'></i> {{ activity.tuesday.content.text | markdownify }}</td>
        {% elsif activity.tuesday %}
          <td><i class='fas fa-{{ activity.tuesday.icon }}'></i> {{ activity.tuesday.text | markdownify }}</td>
        {% endif %}
        {% if activity.wednesday.content %}
          <td rowspan="{{ activity.wednesday.rowspan }}"><i class='fas fa-{{ activity.wednesday.content.icon }}'></i> {{ activity.wednesday.content.text | markdownify }}</td>
        {% elsif activity.wednesday %}
          <td><i class='fas fa-{{ activity.wednesday.icon }}'></i> {{ activity.wednesday.text | markdownify }}</td>
        {% endif %}
        {% if activity.thursday.content %}
          <td rowspan="{{ activity.thursday.rowspan }}"><i class='fas fa-{{ activity.thursday.content.icon }}'></i> {{ activity.thursday.content.text | markdownify }}</td>
        {% elsif activity.thursday %}
          <td><i class='fas fa-{{ activity.thursday.icon }}'></i> {{ activity.thursday.text | markdownify }}</td>
        {% endif %}
        {% if activity.friday.content %}
          <td rowspan="{{ activity.friday.rowspan }}"><i class='fas fa-{{ activity.friday.content.icon }}'></i> {{ activity.friday.content.text | markdownify }}</td>
        {% elsif activity.friday %}
          <td><i class='fas fa-{{ activity.friday.icon }}'></i> {{ activity.friday.text | markdownify }}</td>
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
        {% assign sorted_speakers = site.data.speaker-cards | sort: "surname" %}
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