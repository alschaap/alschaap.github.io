---
layout: page
title: Student  Projects
permalink: /student_projects/
toggle: on
rank: 8
---

### Student Projects

<div class="lab-wrapper">
    <ul class="lab-list">
    {% for project in site.data.student_projects %}
    {% if project.name and project.description %}
        <li>
            <h2>{{ student_projects.name }}</h2>
            {% if student_projects.photo %}
                <img class="float-right projects-photo" src="{{ student_projects.photo | prepend: site.images_dir | prepend: site.baseurl }}">
            {% endif %}
            {% if project.funding %}
                <p><b>Funding: </b>{{ student_projects.funding }}</p>
            {% endif %}
            {% if student_projects.collaborators %}
                <p><b>Collaborators: </b>{{ student_projects.collaborators }}</p>
            {% endif %}
            {% if student_projects.assignees %}
                <p><b>Assignees: </b>{{ student_projects.assignees }}</p>
            {% endif %}
            <p>{{ student_projects.description }}</p>
        </li>
    {% endif %}
    {% endfor %}
    </ul>
</div>
