---
layout: default
permalink: /
---
{% include page-title.html %}

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
            {% include star-rating.html stars=3 %}
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