---
layout: default
title: Home
customjs: shortpubs
---

<div class="container">
    <div class="row">
        <div class="col-md-4">
            <img src="{{ site.baseurl }}/public/images/BeFunky.jpg" width="200px" /><br>  
            Associate Professor (since Sep'16) <br>
            <a href="http://www.cs.sfu.ca">School of Computing Science</a> <br>
            <a href="http://www.sfu.ca">Simon Fraser University</a> <br>
            Email: <code><span class="rev">ac.ufs.sc.@marirhsa</span></code> <br>
            Gmail: <code><span class="rev">moc.liamg@krow.marirhsa</span></code><br>
            <div class="button-group">
                <a href="https://scholar.google.ca/citations?user=ZuBFPTcAAAAJ&hl=en" class="button">Google Scholar</a>
                <a href="https://github.com/ashriram" class="button">Github</a>
                <a href="https://ca.linkedin.com/in/ashriram" class="button">Linkedin</a>
                <a href="https://github.com/sfu-arch" class="button">Group Github</a>

            </div>
        </div>
        <div class="col-md-5">
            <div style="white-space: pre-wrap;">
                Arrvindh Shriraman
                School of Computing Science
                ASB 9241, 8888 University Drive
                Simon Fraser University
                Burnaby, BC V5A 1S6, Canada
                Tel: I prefer email contact.
                <a href="{{ site.baseurl }}/Calendar">
                 <i class="material-icons" style="display:inline-block;" style="font-size:36px">perm_contact_calendar</i>Calendar</a>
                <a href="http://www.sfu.ca/campuses/maps-and-directions/burnaby-map.html"><i class="material-icons" style="font-size:36px">directions_car</i>Directions</a>
               <div style="display:inline-block;" id="SkypeButton_Call_arrvindhshriraman_1"></div>
            </div>
        </div>

<!-- <div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/news">more...</a></li>
        <li><a href="{{ site.baseurl }}/tags">Sorted by tags</a></li>
    </ul>
</div>
   -->
   <div class="col-md-3">

<h3 id="teaching">Teaching</h3>
<ul>
  <li> <a href="{{ site.baseurl }}/Courses/CS295/">295: Intro to Computer Systems </a></li>
</ul>

<h3> Posts </h3>
<ul class="posts">
  {% for post in site.posts limit:2 %}
    {% unless post.draft == 'true' %}
      <li>
        <a href="{{ site.baseurl }}{{ post.url }}">
          <div>
            <span class="title">{{ post.title }}</span>
        </div>
        </a>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
</div>

    </div>

</div>

<div class="alert alert-info">
If you are interested in working with me, before you email me, please read my <a href="{{ site.baseurl }}/firstcontact">First Contact</a> guide.
</div>

<!-- <div id="slider">
    <img src="{{ site.baseurl }}/public/images/BeFunky.jpg" alt="Slide 1" />
    <img data-src="{{ site.baseurl }}/public/images/BeFunky.jpg" alt="Slide 2" />
    <img data-src="{{ site.baseurl }}/public/images/BeFunky.jpg" alt="Slide 3" />
    <script src="{{ site.baseurl }}/public/js/images.js"></script>
</div>
 -->

### Active Research <a href="{{ site.baseurl }}/research">(more-)</a>

<img src="{{ site.baseurl }}/public/images/research_wordle_black.png" width="50%" /><br>

<table class="table">
{% for research in site.data.research %}
    <tr>
        <td>
            <b>{{ research.name }}</b>
<img src="{{ site.baseurl }}/public/images/{{ research.picture }}" width="100px" />  </td>
<td>
 <span class="smaller"> {{ research.description }} </span>
        <!-- <ul class="smaller"><li>After: {{ postdoc.after }}</li></ul> -->
    </td>
</tr>
{% endfor %}
</table>

<!-- * Hardware accelerators -->
<!-- //* Cache Coherence and Memory Hierarchy -->
<!-- * Parallelism and Synchronization -->
<!-- //* Energy Efficiency -->

<!--
<p><span class="moreinfo"><a href="{{ site.baseurl }}/news">All news and posts ...</a></span></p>
-->

### Recent Publications and Talks

<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/publications/index.html">All publications</a></li>
    </ul>
</div>

{% include shortpubs.html %}

### Software

<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/software/index.html">All software</a></li>
    </ul>
</div>

{% include software.html param=2 %}

### Service (<a href="{{ site.baseurl }}/service">more-</a>)

- Program committee members, ASPLOS 2017, MICRO 2016, HPCA 2015,
- Local Arrangements Chair, MICRO 2012.

### Recently Graduated Students

<div class="more">
    <ul class="navigate">
        <li><a href="{{ site.baseurl }}/people">All students and postdocs</a></li>
        <li><a href="{{ site.baseurl }}/theses">Student theses</a></li>
    </ul>
</div>

{% include graduatedstudents.html param=2 %}

<script src="{{ site.baseurl }}/public/js/ideal-image-slider.js"></script>
<script>
    var slider = new IdealImageSlider.Slider('#slider');
    slider.start();
</script>

<script type="text/javascript" src="https://secure.skypeassets.com/i/scom/js/skype-uri.js"></script>

<script type="text/javascript">
 Skype.ui({
 "name": "chat",
 "element": "SkypeButton_Call_arrvindhshriraman_1",
 "participants": ["arrvindhshriraman"]
 });
</script>
