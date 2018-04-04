---
layout: default
title: Board Family | Blog
permalink: /games/
---
<!-- PAGE TITLE SECTION-->
<section class="pageTitleSection">
  <div class="container">
    <div class="pageTitleInfo">
      <h2>Board Family Blog</h2>
      <ol class="breadcrumb">
        <li><a href="/">Home</a></li>
        <li class="active">Blog</li>
      </ol>
    </div>
  </div>
</section>
<section class="mainContent full-width clearfix coursesSection">
  <div class="container">
    <div class="row">
      {% for post in site.posts %}
      {% assign colorIndex = forloop.index0 | modulo: 6 | plus: 1 %}
      <div class="col-sm-4 col-xs-12 block">
        <div class="thumbnail thumbnailContent">
          <a href="single-blog-left-sidebar.html"><img src="http://via.placeholder.com/270x230" alt="image" class="img-responsive"></a>
          <div class="sticker-round bg-color-{{colorIndex}}">{{ post.date | date: "%-d" }} <br>{{ post.date | date: "%b" }}</div>
          <div class="caption border-color-{{colorIndex}}">
            <h3><a href="single-blog-left-sidebar.html" class="color-{{colorIndex}}">{{ post.title }}</a></h3>
            <ul class="list-inline">
              <li><i class="fa fa-users" aria-hidden="true"></i> {{ post.stats.players }}</li>
              <li><i class="fa fa-child" aria-hidden="true"></i> {{ post.stats.age }}</li>
              <li><i class="fa fa-clock" aria-hidden="true"></i> {{ post.stats.duration }}</li>
            </ul>
            <p>{{ post.description }}</p>
            <ul class="list-inline btn-yellow">
              <li><a href="single-blog-left-sidebar.html" class="btn btn-link"><i class="fa fa-angle-double-right" aria-hidden="true"></i> More</a></li>
            </ul>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>