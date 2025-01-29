---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-full
title: "Home"
show_sidetoc: true
subtitle: "22-28 June 2025 – Baratti (Piombino) – TUSCANY (Italy)"
header_type: hero #base, post, hero,image, splash
header_img: assets/images/poggio.jpg
header_title: "From Data to Social Innovation"
---

<div class="full-width-wrapper">
    <img src="{{ site.baseurl }}/assets/images/header.svg" alt="sbd-pattern" class="full-width-image">
</div>

<div class="introduction">
    <div class="container">
        <div class="row pt-2">
            <div class="col-md-8 offset-md-2 col-sm-12">
               <h3>
The Summer School aims to equip researchers, data scientists and social scientists with the methodologies and insights necessary to address complex societal challenges.
</h3>
                <p class="mt-3"><strong>The school is organised in four thematic days about the:</strong></p>
            </div>
        </div>
    </div>
</div>
<div class="container-fluid my-5">
{% include img-gallery-cards.html 
    datasource='days-description'
    img_url='image'
    name='day'
    description='description'
    container='fluid' 
%}
</div>


<div class="introduction">
    <div class="container">
        <div class="row pt-2">
            <div class="col-md-8 offset-md-2 col-sm-12">
                <p>
                The Summer School provides a unique <strong>interdisciplinary mixture</strong> where participants can explore state-of-the-art tools in <strong>data analysis, machine learning, and artificial intelligence</strong>. The school will have lessons from experts during the morning and will leave the afternoon to <strong>group work guided by dedicated tutors</strong> helping them in defining and developing their project which will be evaluated at the end of the school by a panel of experts.</p>
                <hr>
                <p>
                <strong>Expert-led lectures</strong> will guide attendees through real-world applications of big data and AI, fostering innovative solutions. Alongside technical skill-building, participants engage in <strong>ethical and governance discussions</strong> that highlight the responsible use of data.
                </p>
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
            <p class="lead">Nested in the gulf of Baratti on the “Etruscan Coast” in Tuscany (Italy), <a href="{{ site.baseurl }}{% link _pages/venue.markdown %}">Poggio all’Agnello </a> is a fully equipped resort that will host the 2025 edition of the SoBigData Summer school.
            </p>
            <h3>Registration & Deadline</h3>
            <p>Early registration until 30 April 2025.</p>
            <p><strong>Late registration between 1 May 2025 and 31 May 2025 will have an additional cost.</strong></p>
            </div>
        </div>
    </div>
</div>

<div class="aim mt-5">
    <div class="container">
        <div class="row pt-2 ">
        <div class="col-md-6 col-sm-12">
            <h3>AIM OF THE SCHOOL</h3>
                <p>
                The Summer School aims to equip <strong>researchers, data scientists, and social scientists</strong> with an <strong>interdisciplinary understanding and skill set</strong> to address complex societal challenges. By blending <strong>technical training in data analysis, machine learning, and artificial intelligence</strong> with <strong>ethical, political, and social dynamics</strong>, the program empowers the students in facing today's pressing societal challenges with a balanced approach that combines <strong>innovative data methodologies, stakeholder awareness, and a commitment to responsible, transparent practices</strong>.
                </p>
                <p>
                    Over <strong>four themed days</strong>, participants first explore the <strong>new European research framework</strong>—covering directives, open science principles, and data-sharing policies. Next, they dive into <strong>Information Dynamics</strong>, examining how (dis)information is created, transferred, and transformed. The third focus, <strong>Political Dynamics</strong>, looks at how policy, ideology, institutions, and individuals shape discussions and social discourse. Finally, <strong>Social Dynamics</strong> reveals how communities and institutions influence each other, how societal structures evolve, and how collective behaviors emerge. <strong>Expert-led lectures</strong> throughout the mornings expose participants to state-of-the-art methods and real-world case studies, highlighting best practices and contemporary applications of big data and AI. The <strong>afternoon sessions</strong> are dedicated to <strong>collaborative group projects</strong>, allowing students to actively engage in hands-on learning experiences. At the end of the week, a <strong>panel of experts</strong> in data mining and AI will evaluate the projects. This approach ensures a comprehensive and interactive learning environment allowing the participants to explore the <strong>ethical, legal, and practical dimensions</strong> of leveraging data for societal well-being.
                </p>
            </div>
            <div class="col-md-6 col-sm-12">
            <div class="project lead px-3 py-1">
               <h3>Topics</h3>
                <ul>
                    <li>Data Science</li>
                    <li>Artificial Intelligence</li>
                    <li>Machine Learning</li>
                    <li>Social Network Analysis</li>
                    <li>Data Governance</li>
                    <li>Disinformation</li>
                    <li>Information Dynamics</li>
                    <li>Social Dynamics</li>
                    <li>Political Dynamics</li>
                    <li>Large Language Models</li>
                    <li>Sustainable Development</li>
                    <li>Open Science</li>
                    <li>Data Altruism</li>
                </ul>
            </div>
            <div class="project lead px-3 py-1 mt-2">   
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

<div class=" container-fluid my-5 pt-2 pb-5 bg-color-full bg-color">
    <div class="container">
        <div class="row">
            <div class="col-md-12">
                <h3 class="text-white">Keynote Speakers</h3>
                <hr>
            </div>
        </div>
    </div>
{% include img-gallery-cards.html  
    datasource='speaker-cards' 
    url='img_url' 
    name='name' 
    description='institution' 
    container='fluid' 
%}
</div>


<div class="container cta">
        <div class="row py-5">
            <div class="col-md-12">
                <div>
                    <h3>Interested in attending?</h3>
                    <a href="{{site.baseurl}}{% link _pages/registration.markdown %}" class="btn btn-primary">Register now</a>
                </div>
            </div>
        </div>
</div>





<div class="container credits pt-5">
    <div class="row">
        <div class="col-md-12">
            <h5>This summer school is organized and supported by</h5>
        <div class="logo-grid">
                    <img src="{{ site.baseurl }}/assets/images/Logo_SoBigData_RI_560_X_100.png" alt="SoBigData RI" >
                    <img src="{{ site.baseurl }}/assets/images/Logo_SoBigData_ITA_560_X_100.png" alt="SoBigData it" >
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
