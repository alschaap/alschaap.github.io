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

###  **Title:** Deep Learning

###  **Title:** Benchmarking neoepitope prediction methods


#### **Aim:** The aim of this project is to


#### **Impact:**


### **Title:** Embedding the immune system

 **Aim:** The aim of this project is to


**Impact:**


### **Title:** The role and effects of partitioning

#### **Aim:** The aim of this project is to identify which partitioning method is the most meaningful for data redundancy and least computationally expensive to obtain the best possible predictions when using Deep Learning.

In sequence analysis, clustering is used to group homologous sequences into gene or protein families.
#### **The project:** The student will be


#### **Aim:**  
Many partitioning methods currently exist, however, it is unclear what their strengths and weaknesses are in regards to biological data.
