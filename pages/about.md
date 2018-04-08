---
layout: default
title: Board Family | About
permalink: /about/
---
{% include page-title.html title="Who We Are" page="About" %}
<section class="mainContent full-width clearfix">
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <div class="sectionTitle text-center">
          <h2>
            <span class="shape shape-left bg-color-4"></span>
            <span>We Love Games</span>
            <span class="shape shape-right bg-color-4"></span>
          </h2>
          <p>Something about games and why we like them.</p>
        </div>
      </div>
    </div>
  </div>
</section>
<section class="mainContent full-width clearfix">
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <div class="sectionTitle text-center">
          <h2>
            <span class="shape shape-left bg-color-4"></span>
            <span>The Parents</span>
            <span class="shape shape-right bg-color-4"></span>
          </h2>
        </div>
      </div>
    </div>
    <div class="row">
      {% include about-parent.html name="Parent 1" title="title" %}
      {% include about-parent.html name="Parent 2" title="title" %}
      {% include about-parent.html name="Parent 3" title="title" %}
      {% include about-parent.html name="Parent 4" title="title" %}
    </div>
  </div>
</section>
<section class="colorSection full-width clearfix bg-color-4 teamSection">
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <div class="sectionTitle text-center alt">
          <h2>
            <span class="shape shape-left bg-color-3"></span>
            <span>The Kids</span>
            <span class="shape shape-right bg-color-3"></span>
          </h2>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-12">
        <div class="owl-carousel teamSlider">
          {% include about-kid.html name="Kid 1" age=10 %}
          {% include about-kid.html name="Kid 2" age=9 %}
          {% include about-kid.html name="Kid 3" age=8 %}
          {% include about-kid.html name="Kid 4" age=7 %}
          {% include about-kid.html name="Kid 5" age=6 %}
          {% include about-kid.html name="Kid 6" age=5 %}
          {% include about-kid.html name="Kid 7" age=4 %}
        </div>
      </div>
    </div>
  </div>
</section>