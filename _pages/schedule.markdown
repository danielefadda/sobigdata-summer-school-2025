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
                <table border="1" cellpadding="8" cellspacing="0">
                    <thead>
                        <tr>
                            <th>TIME</th>
                            <th>Sunday 16</th>
                            <th>Monday 17</th>
                            <th>Tuesday 18</th> 
                            <th>Wednesday 19</th>   
                            <th>Thursday 20</th>    
                            <th>Friday 21</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr class="break">
                            <td>9:00 9:30</td>
                            <td></td>
                            <td>Registration</td>
                            <td></td>
                            <td></td>
                            <td></td>
                            <td></td>
                        </tr>
                        <tr>
                            <td>9:30 10:00</td>
                            <td></td>
                            <td>Round of presentations (Students)</td>
                            <td></td>
                            <td></td>
                            <td></td>
                            <td></td>
                        </tr>
                        <tr>
                            <td>10:00 10:30</td>
                            <td></td>
                            <td>Roberto Trasarti - "SciDaSuite RLS School Introduction"</td>
                            <td>Richard Rogers - "Automated Auditing"</td>
                            <td>Alexandre Barth - "Multivariate convolutional neural networks with error estimates to reconstruct missing data in satellite observations"</td>
                            <td>Maryam Mehrnezhad - "Cybersecurity, privacy, bias, and trust in female-oriented technologies"</td>
                            <td>Katharina Munk - "Resource-Aware Machine Learning"</td>
                        </tr>
                        <tr>
                            <td>10:30 11:00</td>
                            <td></td>
                            <td>Angeliki Tzouganatou - "Fostering Open Science Practices"</td>
                            <td></td>
                            <td></td>
                            <td></td>
                            <td></td>
                        </tr>
                        <tr class="break">
                            <td>11:00 11:30</td>
                            <td></td>
                            <td>Coffee Break</td>
                            <td>Coffee Break</td>
                            <td>Coffee Break</td>
                            <td>Coffee Break</td>
                            <td>Coffee Break</td>
                        </tr>
                        <tr>
                            <td>11:30 12:30</td>
                            <td></td>
                            <td>Giovanni Comandé Data (SSSA) - "Governance AI+ethics"</td>
                            <td>Roberto Pellungrini (SNS) - "Explainable AI and hybrid Decision Making Systems"</td>
                            <td>Angelo Facchini (IMT) - "Tracing two decades of carbon emissions using a network approach"</td>
                            <td>Antinsca Di Marco (UNINA/Q)- "Analyzing health data: from genomic to clinical data"</td>
                            <td>Mark Cole, Massimiliano Assante, Katharina Munk and Richard Rogers "Project Evaluation"</td>
                        </tr>
                        <tr>
                            <td>12:30 13:30</td>
                            <td></td>
                            <td>Mark Cole (VCL) - "Data Altruism: Data for Public Good?"</td>
                            <td>Salvatore Ruggieri "Bias in AI"</td>
                            <td>Franco D. Cicirelli (ICAR)- "Sustainable Cognitive Buildings"</td>
                            <td>Jennifer Pybus (York University) - "Tracking Human Health Using Method for Auditing Menopause App Infrastructure"</td>
                            <td></td>
                        </tr>
                        <tr class="break">
                            <td>13:30 15:00</td>
                            <td></td>
                            <td>Lunch Break</td>
                            <td>Lunch Break</td>
                            <td>Lunch Break</td>
                            <td>Lunch Break</td>
                            <td>Lunch Break</td>
                        </tr>
                        <tr>
                            <td>15:00 18:00</td>
                            <td></td>
                            <td>Developing Student Projects with Tutors</td>
                            <td>Developing Student Projects with Tutors</td>
                            <td>Social Event: trip Populonia</td>
                            <td>Developing Student Projects with Tutors</td>
                            <td>Open discussion for follow-up activities</td>
                        </tr>
                        <tr>
                            <td>18:00</td>
                            <td>Welcome Cocktail</td>
                            <td></td>
                            <td></td>
                            <td></td>
                            <td></td>
                            <td></td>
                        </tr>
                        <tr>
                            <td>20:00</td>
                            <td>Hotel Dinner</td>
                            <td>Hotel Dinner</td>
                            <td>Social program - Winery visit and social dinner</td>
                            <td>Hotel Dinner</td>
                            <td>Social program - Pizza and DJ set</td>
                            <td>Hotel Dinner</td>
                        </tr>
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