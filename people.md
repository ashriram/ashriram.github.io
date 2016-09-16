---
layout: linkedpage
title: People
menu: true
relatedpages:
  - title: "All student theses"
    url: theses
---


## Postdoctoral Fellows

<ul>
{% for postdoc in site.data.postdocs %}
    <li>{{ postdoc.name }} <span class="smaller">({{ postdoc.start }} to {{ postdoc.end }})</span>
        <!-- <ul class="smaller"><li>After: {{ postdoc.after }}</li></ul> -->
    </li>
{% endfor %}
</ul>

## Current Graduate Students

{% include currentstudents.html %}

## Undergraduates


## Graduated Students

{% include graduatedstudents.html %}


## Students Supervised

I served as Supervisor on the thesis committee of these graduated students.

{% include supervisor.html %}

{% comment %}

## Students Examined

I served as Examiner on the thesis committee of these students.

{% include examiner.html %}

{% endcomment %}

{% comment %}
<ul>
{% for ugrad in site.data.undergrads %}
    <li>{{ ugrad.name }}
        <span class="smaller">(
        {% for sem in ugrad.semesters %}
            {{ sem.semester }}
        {% endfor %}
        )
        {% if ugrad.after %}
            &raquo; {{ ugrad.after }}
        {% endif %}
        </span>
        <!--
        <ul class="smaller">
        {% for sem in ugrad.semesters %}
            <li>{{ sem.semester }} (Funding: {{ sem.funding }})</li>
        {% endfor %}
        </li>
        {% if ugrad.after %}
            <li>After: {{ ugrad.after }}</li>
        {% endif %}
        </ul>
        -->
    </li>
{% endfor %}
</ul>

<hr/>
{% endcomment %}