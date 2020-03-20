---
layout: program
title:  "Financial Aid Programme for the Control and <br/>Prevention of COVID-19"
cover: https://img.mayun.xin/upload/2020031723/3e084fc22806bc14657a41b0275a0c5b.jpg?x-oss-process=image/resize,w_1600,limit_0/format,jpg/quality,Q_90/contrast,-60
slogan: 
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
      <p>Since the global outbreak of COVID-19, the Jack Ma Foundation has been supporting those most affected countries. Together with Alibaba Foundation, we have sourced and donated millions of masks and other personal protective equipments. So far, we have donated masks and testing kits to Japan, South Korea, Iran, Italy, Spain, United States and Africa. We hope to continue to promptly deliver these medical supplies to those in need, and wish to offer our sincere thanks to all countries who have helped us.</p>
    </div>
  </section>

  <section class="odd">
    <div class="section-heading"><h2>Donation Details</h2></div>
    <div class="section-body container aids">

      <div class="panel-group panel-supplies-group" id="accordion" role="tablist" aria-multiselectable="true">
        {% for item in site.data.supplies %}
        <div class="panel panel-default panel-country">
            <div class="panel-heading" role="tab" id="heading-{{ forloop.index }}">
                <h4 class="panel-title">
                    <a role="button" data-toggle="collapse" data-parent="#accordion" href="#collapse-{{ forloop.index }}"  aria-controls="collapse-{{ forloop.index }}">
                    <div class="country-name"><i class="fa fa-caret-down toggle-indicator-icon" aria-hidden="true"></i>{{ item.country }}</div>
                    <!-- <div class="state">DONE</div> -->
                    </a>
                </h4>
            </div>
            <div id="collapse-{{ forloop.index }}" class="panel-collapse collapse" role="tabpanel" aria-labelledby="heading-{{ forloop.index }}">
                <div class="panel-body">
                    {% for supply in item.supplies %}
                      <div class="supply-item">
                        <div class="line">
                            <span class="label">Goods</span>
                            <span class="value">{{ supply.goods }}</span>
                        </div>
                        <div class="line">
                            <span class="label">QTY(Piece)</span>
                            <span class="value">{{ supply.qty }}</span>
                        </div>
                        <div class="line">
                            <span class="label">Progress</span>
                            <span class="value">{{ supply.progress }}</span>
                        </div>
                        <div class="line">
                            <span class="label">Recepient</span>
                            <span class="value">{{ supply.recepient }}</span>
                        </div>
                      </div>
                      {% if forloop.index!=forloop.length %}
                        <hr/>
                      {% endif %} 
                    {% endfor %} 
                </div>
            </div>
        </div> 
        {% endfor %} 
      </div>



      {% for item in site.data.supplies %}
      <div class="aid">
        <div class="country">{{ item.country }}</div>
        <table>
          <thead>
            <tr>
              <th class="c2">Goods</th>
              <th class="c1" style="text-align: right">QTY(Piece)</th>
              <th class="c2">Progress</th>
              <th>Recepient</th>
            </tr>
          </thead>
          <tbody>
            {% for supply in item.supplies %}
            <tr>
              <td>{{ supply.goods }}</td>
              <td style="text-align: right">{{ supply.qty }}</td>
              <td>{{ supply.progress }}</td>
              <td>{{ supply.recepient }}</td>
            </tr>
            {% endfor %} 
          </tbody>
        </table>
      </div>
      {% endfor %} 

      <p>Note：</p>
      <p>Detection Kit：Detection Kit for 2019 Novel Coronavirus(COVID-19)RNA(PCR-Fluorescence Probing)</p>
      <p>Nucleic Acid Isolation or Purification Reagent: Used for steps of extraction, enrichment, purification,etc.of nucleic acid. Its processed product is used for clinical in vitro detection.</p>
      <p>NAT：is intended for the collection and preservation of clinical specimens containing viruses or other pathogens.</p>
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