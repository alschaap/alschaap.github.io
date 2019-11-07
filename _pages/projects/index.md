---
layout: page
title: Projects
permalink: /projects/
toggle: on
rank: 1
---



<div class="lab-wrapper">
    <ul class="lab-list">
    {% for project in site.data.projects %}
    {% if project.name and project.description %}
        <li>
            <h2>{{ project.name }}</h2>
            {% if project.photo %}
                <img class="float-right projects-photo" src="{{ project.photo | prepend: site.images_dir | prepend: site.baseurl }}">
            {% endif %}
            {% if project.funding %}
                <p><b>Funding: </b>{{ project.funding }}</p>
            {% endif %}
            {% if project.collaborators %}
                <p><b>Collaborators: </b>{{ project.collaborators }}</p>
            {% endif %}
            {% if project.assignees %}
                <p><b>Assignees: </b>{{ project.assignees }}</p>
            {% endif %}
            <p>{{ project.description }}</p>
        </li>
    {% endif %}
    {% endfor %}
    </ul>
</div>


## **Student Projects**

### **Title:** The role and effects of partitioning

#### **Aim:** The aim of this project is to identify which partitioning method is the most meaningful for data redundancy and least computationally expensive to obtain the best possible predictions when using Deep Learning.

#### **The project:** The student will be working with different partitioning methods to study their effect and role in Deep Learning predictions.

###  **Title:** Benchmarking neoepitope prediction methods

###  **Title:** Deep Learning for CDR3 structural feature predictions

###  **Title:** The effect of checkpoint inhibitor therapy on lymphocyte repertoire composition

###  **Title:** Lyra 2.0: furtherance of existing template based prediction

###  **Title:** Developing a similarity metric for complementarity (Taken)

###  **Title:** Diversity of TCR repertoires: state of the art and prospects

### **Title:** Embeddings for the immune system

### **Title:** Chronic lymphatic leukemia
