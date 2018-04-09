---
layout: default
title: About
permalink: /about/
---
{% include page-title.html title="Who We Are" page="About" %}
<section class="mainContent full-width clearfix aboutSection">
  <div class="container">
    <div class="row">
      <div class="col-sm-6 col-sm-push-6 col-xs-12">
        <img src="//via.placeholder.com/540x440" alt="image" class="img-responsive img-rounded">
      </div>
      <div class="col-sm-6 col-sm-pull-6 col-xs-12">
        <div class="schoolInfo">
          <h2>Welcome to The Board Family</h2>
          <p>
            We love to play games, and it doesn't matter the age level, difficulty or genre.
            We also have kids and recognize that not every game is suitable for a family game night depending on the mix of ages in the family.
          </p>
          <p class="color-3">At The Board Family we strive to provide fun and honest reviews</p>
          <ul class="list-unstyled para-list">
            <li><i class="fa fa-check" aria-hidden="true"></i> Vestibulum iaculis quam ac libero volutpat placerat.</li>
            <li><i class="fa fa-check" aria-hidden="true"></i> Phasellus sit amet risus fringilla, aliquet lacus vel, suscipit lorem.</li>
            <li><i class="fa fa-check" aria-hidden="true"></i> Etiam suscipit velit et tellus bibendum interdum.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>
<section class="colorSection full-width clearfix bg-color-4 servicesSection bg-pattern-light">
  <div class="container">
    <div class="sectionTitle text-center alt">
      <h2>
        <span class="shape shape-left bg-color-3"></span>
        <span>How We Review a Game</span>
        <span class="shape shape-right bg-color-3"></span>
      </h2>
    </div>
    <div class="row">
      <div class="col-sm-4 col-sm-offset-2 col-xs-12">
        <div class="media servicesContent rightAlign">
          <a class="media-left" href="service-details.html">
            <i class="fa fa-graduation-cap" aria-hidden="true"></i>
          </a>
          <div class="media-body">
            <h3 class="media-heading">Teachability</h3>
            <p>Is it easy to learn, or will I be constantly in the rule book?</p>
          </div>
        </div>
        <div class="media servicesContent rightAlign">
          <a class="media-left" href="service-details.html">
            <i class="fa fa-calendar-check" aria-hidden="true"></i>
          </a>
          <div class="media-body">
            <h3 class="media-heading">Real Age</h3>
            <p>The box says 12+, but can my 8 year old daughter play?</p>
          </div>
        </div>
      </div>
      <div class="col-sm-4 col-xs-12">
        <div class="media servicesContent">
          <a class="media-left" href="service-details.html">
            <i class="fa fa-sync-alt" aria-hidden="true"></i>
          </a>
          <div class="media-body">
            <h3 class="media-heading">Replayability</h3>
            <p>Does it pass the "Can we play again even though I lost" test?</p>
          </div>
        </div>
        <div class="media servicesContent">
          <a class="media-left" href="service-details.html">
            <i class="fa fa-clock" aria-hidden="true"></i>
          </a>
          <div class="media-body">
            <h3 class="media-heading">Real Play Time</h3>
            <p>How long does it <em>actually</em> take to play with setup and cleanup?</p>
          </div>
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
            <span>Meet The Parents</span>
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
<section class="colorSection full-width clearfix bg-color-3 teamSection bg-pattern-light">
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <div class="sectionTitle text-center alt">
          <h2>
            <span class="shape shape-left bg-color-4"></span>
            <span>Meet The Kids</span>
            <span class="shape shape-right bg-color-4"></span>
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