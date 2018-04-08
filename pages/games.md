---
layout: default
title: Board Family | Games
permalink: /games/
---
{% include page-title.html page="Games" %}

<section class="mainContent full-width clearfix">
  <div class="container">
    <div class="row">
      <!-- <div class="col-md-3 col-md-push-9 col-sm-5 col-sm-push-7 col-xs-12">
        <aside>
          <div class="panel panel-default courseSidebar">
            <div class="panel-heading bg-color-1 border-color-1">
              <h3 class="panel-title">Search</h3>
            </div>
            <div class="panel-body">
              <div class="input-group">
                <input type="text" class="form-control" placeholder="Enter Your Search" aria-describedby="basic-addon2">
                <span class="input-group-addon" id="basic-addon2"><input class="btn btn-primary bg-color-1" type="submit" value="Search"></span>
              </div>
            </div>
          </div>
          <div class="panel panel-default courseSidebar">
            <div class="panel-heading bg-color-2 border-color-2">
              <h3 class="panel-title">Filter By</h3>
            </div>
            <div class="panel-body">
              <div class="lightDrop">
                <select name="guiest_id4" id="guiest_id4" class="select-drop">
                  <option value="0">All Classes</option>
                  <option value="1">One</option>
                  <option value="2">Two</option>
                  <option value="3">Three</option>
                </select>
              </div>
              <div class="lightDrop">
                <select name="guiest_id5" id="guiest_id5" class="select-drop">
                  <option value="0">Ages</option>
                  <option value="1">3</option>
                  <option value="2">4</option>
                  <option value="3">5</option>
                </select>
              </div>
              <div class="priceRange">
                <div class="price-slider-inner">
                  <span class="amount-wrapper">
                    Price:
                    <input type="text" id="price-amount-1" readonly>
                    <strong>-</strong>
                    <input type="text" id="price-amount-2" readonly>
                  </span>
                  <div id="price-range"></div>
                </div>
                <input class="btn btn-primary bg-color-2" type="submit" value="Filter">
              </div>
            </div>
          </div>
        </aside>
      </div> -->
      <div class="col-12">
        {% assign sortedPosts = site.posts | sort: 'title' %}
        {% for post in sortedPosts %}
        {% assign colorIndex = forloop.index0 | modulo: 6 | plus: 1 %}
        <div class="media courseList couresListPage">
          <a class="media-left border-color-{{colorIndex}}" href="{{post.url}}">
            <img class="media-object" src="http://via.placeholder.com/270x200" alt="Image">
          </a>
          <div class="media-body">
            <h3 class="media-heading"><a href="{{post.url}}" class="color-{{colorIndex}}">{{ post.title }}</a></h3>
            <ul class="list-inline">
              <li><i class="fa fa-users" aria-hidden="true"></i> {{ post.stats.players }}</li>
              <li><i class="fa fa-child" aria-hidden="true"></i> {{ post.stats.age }}</li>
              <li><i class="fa fa-clock" aria-hidden="true"></i> {{ post.stats.duration }}</li>
            </ul>
            <p>{{ post.description }}</p>
            <ul class="list-inline btn-color-{{colorIndex}} btnPart">
              <li><a href="{{post.url}}" class="btn btn-link pl0"><i class="fa fa-angle-double-right" aria-hidden="true"></i> More</a></li>
            </ul>
          </div>
        </div>
        {% endfor %}
      </div>
    </div>
  </div>
</section>