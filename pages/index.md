---
layout: default
permalink: /
---
<!-- BANNER -->
<section class="bannercontainer bannercontainerV1">
  <div class="fullscreenbanner-container">
    <div class="fullscreenbanner">
      <ul>
        <li data-transition="fade" data-slotamount="5" data-masterspeed="1000" data-title="Slide 2">
          <img src="//via.placeholder.com/1920x720" alt="slidebg1" data-bgfit="cover" data-bgposition="center center" data-bgrepeat="no-repeat">
          <div class="slider-caption container">
            <div class="tp-caption rs-caption-1 sft start text-center"
              data-hoffset="0"
              data-x="center"
              data-y="200"
              data-speed="800"
              data-start="1000"
              data-easing="Back.easeInOut"
              data-endspeed="300">
              The Board Family
            </div>
            <div class="tp-caption rs-caption-2 sft text-center"
              data-hoffset="0"
              data-x="center"
              data-y="265"
              data-speed="1000"
              data-start="1500"
              data-easing="Power4.easeOut"
              data-endspeed="300"
              data-endeasing="Power1.easeIn"
              data-captionhidden="off">
              Real board game reviews with the whole family in mind
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</section>

<!-- CONTENT -->
<section class="whiteSection full-width clearfix coursesSection" id="ourCourses">
  <div class="container">
    <div class="sectionTitle text-center">
      <h2>
        <span class="shape shape-left bg-color-4"></span>
        <span>Latest Reviews</span>
        <span class="shape shape-right bg-color-4"></span>
      </h2>
    </div>
    <div class="row">
      {% for post in site.posts limit: 4 %}
      {% assign colorIndex = forloop.index0 | modulo: 6 | plus: 1 %}
      <div class="col-sm-3 col-xs-12 block">
        <div class="thumbnail thumbnailContent">
          <a href="{{post.url}}"><img src="//via.placeholder.com/270x230" alt="image" class="img-responsive"></a>
          <div class="caption border-color-{{colorIndex}}">
            <h3><a href="{{post.url}}" class="color-{{colorIndex}}">{{ post.title }}</a></h3>
            {% include star-rating.html stars=post.stars %}
            <ul class="list-inline btn-color-{{colorIndex}}">
              <li><a href="{{post.url}}" class="btn btn-link pl0"><i class="fa fa-angle-double-right" aria-hidden="true"></i> More</a></li>
            </ul>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>