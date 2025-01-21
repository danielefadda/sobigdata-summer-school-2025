---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-full
title: "Home"
show_sidetoc: true
subtitle: "22-28 June 2025, Baratti – TUSCANY (Italy)"
header_type: hero #base, post, hero,image, splash
header_img: assets/images/poggio.jpg
header_title: "From Data to Social Innovation"
---

<div class="full-width-wrapper">
    <img src="{{ site.baseurl }}/assets/images/header.svg" alt="sbd-pattern" class="full-width-image">
</div>

<div class="introduction">
    <div class="container">
        <div class="row pt-2 ">
            <div class="col-md-8 offset-md-2 col-sm-12">
               <p class="lead" style="text-align:justify">The Summer School aims to equip researchers, data scientists and social scientists with the methodologies and insights necessary to address complex societal challenges. Focusing on issues related to <strong>disinformation</strong>, <strong>political dynamics</strong>, and <strong>disaster response</strong>, the Summer School provides a unique interdisciplinary mixture where participants can explore state-of-the-art tools in data analysis, machine learning, and data visualization.
                </p>
                <hr>
                <p>Expert-led lectures will guide attendees through real-world applications of big data and AI, fostering innovative solutions for combating disinformation, understanding and predicting political trends, and improving strategies for disaster risk reduction. Alongside technical skill-building, participants engage in ethical and governance discussions that highlight the responsible use of data.
                The Students will develop their own project during the week collaborating with each other in groups.
                </p>
                <hr>
            </div>
        </div>
    </div>

</div>

<div class="where">
    <div class="container">
        <div class="row pt-2 ">
            <div class="col-md-6 col-sm-12">
               <img src="{{ site.baseurl }}/assets/images/poggio-allagnello.jpeg" alt="Poggio all'Agnello">
            </div>
        <div class="col-md-6 col-sm-12">
            <h3>WHERE</h3>
            <p class="lead">Nested in the gulf of Baratti on the “Etruscan Coast” in Tuscany (Italy), <a href="https://www.poggioallagnello.it/en/">Poggio all’Agnello </a> is a fully equipped resort that will host the 2025 edition of the SoBigData Summer school.
            </p>
            <h3>Registration & Deadline</h3>
            <p>Early registration until Tuesday 30 April 2025.</p>
            <p><strong>Late registration between Wednesday 1 May 2024 and Friday 31 May 2024 will have an additional cost.</strong> There are different fee options, please see the Registration page for details.</p>
            </div>
        </div>
    </div>
</div>

<div class="aim mt-5">
    <div class="container">
        <div class="row pt-2 ">
        <div class="col-md-6 col-sm-12">
            <h3>AIM OF THE SCHOOL</h3>
            <p>Data science and artificial intelligence (AI) play an increasingly important role in our daily lives. AI and its applications are essential tools for the advancement of our multicultural and interconnected society. However, the utilization of these technologies necessitates a thoughtful examination of the ethical and legal dimensions governing data use. The “Empowering Data for Social Good” school is designed to acquaint participants with pivotal subjects, including data governance and trustworthy AI, with a particular focus on applications related to health and sustainable development. To give students the opportunity to actively participate, the school is organized in two sections: the morning sessions feature presentations by accomplished experts, each specializing in the varied topics covered. Concurrently, the afternoon sessions are dedicated to collaborative group projects, allowing students to actively engage in hands-on learning experiences. At the end of the week, a panel of experts in data mining and AI will evaluate the projects. The students will have the flexibility to self-organize their project work time, enabling interaction with tutors for guidance, inquiries, and discussions pertaining to project objectives. This approach ensures a comprehensive and interactive learning environment allowing the participants to explore the ethical, legal, and practical dimensions of leveraging data for societal well-being.</p>
            </div>
            <div class="col-md-6 col-sm-12 project lead">
               <h3>Topics</h3>
                <ul>
                    <li>Data Science</li>
                    <li>Artificial Intelligence</li>
                    <li>Trustworthy AI</li>
                    <li>Explainable AI</li>
                    <li>Neural Networks</li>
                    <li>Machine Learning</li>
                    <li>Data Governance</li>
                    <li>Health and Data</li>
                    <li>Sustainable Development</li>
                </ul>
                <h3>Target attendees</h3>
                <ul>
                    <li>Postgraduate Students</li>
                    <li>PhD Students</li>
                    <li>Researchers</li>
                    <li>Social Scientists</li>
                </ul>
            </div>
        </div>
    </div>
</div>

<div class="container py-3" id="projects-container">
        <h3>Keynote speakers</h3>   
        {% for speaker in site.data.speaker-cards %}
            {% if speaker.home == true %}
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
            {% endif %}
        {% endfor %}
</div>
<div class="container cta">
        <div class="row py-5">
            <div class="col-md-12">
                <div>
                    <h3>Interested in attending?</h3>
                    <a href="{{site.baseurl}}/registration" class="btn btn-primary">Register now</a>
                </div>
            </div>
        </div>
</div>





<div class="container credits pt-5">
    <div class="row">
        <div class="col-md-12">
            <h5>This summer school is organized and supported by</h5>
        <div class="logo-grid">
                    <img src="{{ site.baseurl }}/assets/images/Logo_SoBigData_SC_560_X_100.png" alt="SoBigData it" >
                    <img src="{{ site.baseurl }}/assets/images/fondazioneAREA.png" alt="Fondazione area" >
        </div>
        </div>
    </div>
</div>


<div class="container py-5">
    <div class="row">
        <div class="col-md-12">
            <img src="{{ site.baseurl }}/assets/images/sbd_it_footer.jpg" alt="SoBigDataFooter" class="full-width-image">
        </div>
    </div>
</div>
