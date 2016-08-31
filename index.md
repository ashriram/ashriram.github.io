---
layout: default
title: Home
customjs: shortpubs
---

* [Associate Professor]({{ site.baseurl }})
* [School of Computing Science](http://www.cs.sfu.ca/)
* [Simon Fraser University](http://www.sfu.ca)
{: .contact}

<p>
<div class="button-group">
    <a href="https://scholar.google.ca/citations?user=ZuBFPTcAAAAJ&hl=en" class="button">Google Scholar</a>
    <a href="https://github.com/ashriram" class="button">Github</a>
</div>
</p>


<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/biography">Biography</a></li>
        <li><a href="{{ site.baseurl }}/contact">Contact details</a></li>
    </ul>
</div>

<p>
<div class="alert alert-info">
If you are interested in working with me, before you email me, please read my <a href="{{ site.baseurl }}/firstcontact">First Contact</a> guide.
</div>
</p>

### Research
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/research">More on research</a></li>
    </ul>
</div>

* Hardware acceleratorslerators
* Cache Coherence and Memory Hierarchy
* Parallelism and Synchronization
* Energy Efficiency

### News and Posts
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/news">All news and posts</a></li>
        <li><a href="{{ site.baseurl }}/tags">Sorted by tags</a></li>
    </ul>
</div>

<ul class="posts">
  {% for post in site.posts limit:2 %}
    {% unless post.draft == 'true' %}
      <li>
        <a href="{{ site.baseurl }}{{ post.url }}">
          <div>
            <span class="title">{{ post.title }}</span>
            <span class="date">{{ post.date | date_to_string }}</span>
          </div>
        </a>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
<!--
<p><span class="moreinfo"><a href="{{ site.baseurl }}/news">All news and posts ...</a></span></p>
-->

### Teaching
<!--
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/teaching">All teaching</a></li>
    </ul>
</div>
-->

* Summer 2016: [Compilers](http://anoopsarkar.github.io/compilers-class/)
* Spring 2015: [Machine Learning for Decipherment](http://anoopsarkar.github.io/decipherment-class/)
* Fall 2014: [Natural Language Processing](http://anoopsarkar.github.io/nlp-class/)

### Recent Publications and Talks
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/publications">All publications</a></li>
    </ul>
</div>

{% include shortpubs.html %}

### Software
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/software">All software</a></li>
    </ul>
</div>

{% include software.html param=2 %}

### Research Grants
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/grants">All grants</a></li>
    </ul>
</div>

* IBM Faculty Research Award, 2014-2015.
* NSERC Early Career Award, 2011-2016

### Service
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/service">All activities</a></li>
    </ul>
</div>
* Program committee members, ASPLOS 2017, MICRO 2016, HPCA 2015, 
* Local Arrangements Chair, MICRO 2012.

### Recently Graduated Students
<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/people">All students and postdocs</a></li>
        <li><a href="{{ site.baseurl }}/theses">Student theses</a></li>
    </ul>
</div>

{% include graduatedstudents.html param=2 %}

