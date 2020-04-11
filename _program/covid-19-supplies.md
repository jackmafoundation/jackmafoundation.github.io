---
layout: program
title: "Financial Aid Programme for the Control and <br/>Prevention of COVID-19"
cover: https://img.mayun.xin/upload/2020031723/3e084fc22806bc14657a41b0275a0c5b.jpg?x-oss-process=image/resize,w_1600,limit_0/format,jpg/quality,Q_90/contrast,-60
slogan: 
last_modified_at: 2020-03-20 22:05:17 +0008
permalink: /program/covid-19/supplies
---


<div class="page-ncov">

<div class="banner program-banner" style="background-image: url('{{page.cover}}');">
	<div class="banner-content">
		<div class="container" >
			<h2>{{ page.title }}</h2>
			<p>{{ page.slogan }}</p>
		</div>
	</div>
</div>

<div class="container ncov-nav-tabs">
  <a class="tab" href="/program/covid-19/fund" id="tab-research" data-target="research">
    <h2>Fund on COVID-19 Research, Prevention and Treatment</h2>
  </a>
  <a class="tab active" id="tab-supplies" data-target="supplies">
    <h2>Donation of Medical Supplies for the Control and Prevention of COVID-19</h2>
  </a>
</div>

<div class="program-panel active supplies">

  <section class="even" style="padding-top: 0">
    <div class="section-heading"><h2>Brief Introduction</h2></div>
    <div class="section-body container">
      <p>Months ago, we already experienced the difficulties of epidemic control that other countries are facing now. The Jack Ma Foundation knows very well what China needed and what was insufficient at the time, and these happen to be the urgent-needed supplies by many countries today. </p>
      <p>From sourcing supplies from around the world to China, to raising and delivering supplies to more than 140 countries of five continents together with the Alibaba Foundation, we have always based our donation decisions on the actual development of the pandemic in different regions. We have been adjusting the types and quantities of the donated supplies to meet the practical needs and resolve difficulties truly. </p>
      <p>Time is life. Ensuring there are sufficient medical supplies is critical, and we can’t wait under such circumstances. Every time we raise a batch of supplies, we ship them out as fast as we can.</p>
      <p>One World, One Fight！</p>
    </div>
  </section>

  <section class="even">
    <div class="section-heading"><h2>Related News</h2></div>
    <div class="section-body container">
      <div class="row">
      {% assign counter=0 %}
      {% for post in site.posts %}
        {% if post.tags contains "COVID-19-Supplies" %}
          {% assign counter=counter | plus:1 %}
          <div class="col-md-4">
            <a class="news-card" href="{{ post.url }}" >
              <div class="cover" style="background-image: url('{{ post.cover }}?x-oss-process=image/resize,w_400/');"></div>
              <div class="content">
              <div class="title">{{ post.title }}</div>
              <p class="date">{{ post.date | date: "%Y-%m-%d" }}</p>
              </div>
            </a>
          </div>
          {% if counter == 6%}
            {% break %}
          {% endif %}
        {% endif %}
      {% endfor %}
      </div>
    </div>
  </section>
</div>

</div>