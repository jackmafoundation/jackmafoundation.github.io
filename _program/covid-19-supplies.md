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
      <p>Since the global outbreak of novel coronavirus, the Jack Ma Foundation has been helping the most affected countries. Partner with Alibaba Foundation, we have sourced and donated many masks and other personal protective equipment (PPE). So far, we have donated masks and testing kits to Japan, South Korea, Iran, Italy, Spain, United States, and Africa. We hope to continue to promptly deliver these medical supplies to those in need, and wish to offer our sincere thanks to all countries who have helped us.</p>
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



      <div class="aid">
        <div class="country">Japan</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">300,000</td>
              <td style="text-align: right;">Arrived</td>
              <td style="text-align: right;">ALOGJAPAN CO.,LTD</td>
            </tr>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">1,000,000</td>
              <td style="text-align: right;">Accepted</td>
              <td style="text-align: right;">Nippon Global Medical Organization</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="aid">
        <div class="country">Republic of Korea</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">1,000,000</td>
              <td style="text-align: right;">Accepted</td>
              <td style="text-align: right;">Korean Red Cross</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="aid">
        <div class="country">Islamic Republic of Iran</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">1,000,000</td>
              <td style="text-align: right;">Accepted</td>
              <td style="text-align: right;">Ministry of Foreign Affairs(Iran)</td>
            </tr>
            <tr>
              <td>Detection Kit</td>
              <td style="text-align: right;">100,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Ministry of Foreign Affairs(Iran)</td>
            </tr>
            <tr>
              <td>Nucleic Acid Isolation or Purification Reagent</td>
              <td style="text-align: right;">30,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Ministry of Foreign Affairs(Iran)</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="aid">
        <div class="country">Europe</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">2,000,000</td>
              <td style="text-align: right;">Initial and Second Shipment [Accepted]<br/>The Rest [In Transit]</td>
              <td style="text-align: right;">Italian Red Cross, <br/>Health Management Institute(INGESA) of the Ministry of Health of the Kingdom of Spain</td>
            </tr>
            <tr>
              <td>Detection Kit</td>
              <td style="text-align: right;">200,000</td>
              <td style="text-align: right;">Initial and Second Shipment [Accepted]<br/>The Rest [In Transit]</td>
              <td style="text-align: right;">Sciensano(Belgian institute for health)</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="aid">
        <div class="country">The United States</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">1,000,000</td>
              <td style="text-align: right;">Accepted</td>
              <td style="text-align: right;">Strategic National Stockpile U.S. Department of Health and Human Services</td>
            </tr>
            <tr>
              <td>Detection Kit</td>
              <td style="text-align: right;">500,000</td>
              <td style="text-align: right;">300,000 Detection Kits [In Transit]，<br/>The Rest [Arrived]</td>
              <td style="text-align: right;">Strategic National Stockpile U.S. Department of Health and Human Services</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="aid">
        <div class="country">Republic of Rwanda</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Detection Kit</td>
              <td style="text-align: right;">30,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Rwanda Biomedical Centre </td>
            </tr>
            <tr>
              <td>Nucleic Acid Isolation or Purification Reagent</td>
              <td style="text-align: right;">30,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Rwanda Biomedical Centre </td>
            </tr>
            <tr>
              <td>NAT</td>
              <td style="text-align: right;">30,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Rwanda Biomedical Centre </td>
            </tr>
          </tbody>
        </table>

        
      </div>
      <div class="aid">
        <div class="country">Africa</div>
        <table>
          <thead>
            <tr>
              <th class="column-3">Goods</th>
              <th style="text-align: right;">QTY(Piece)</th>
              <th style="text-align: right;">Progress</th>
              <th class="column-3" style="text-align: right;">Recepient</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Face Mask</td>
              <td style="text-align: right;">6,000,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Recepient to be determined</td>
            </tr>
            <tr>
              <td>Detection Kit</td>
              <td style="text-align: right;">1,100,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Recepient to be determined</td>
            </tr>
            <tr>
              <td>Medical use Protective Suit</td>
              <td style="text-align: right;">60,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Recepient to be determined</td>
            </tr>
            <tr>
              <td>Medical use Protective Face Shield</td>
              <td style="text-align: right;">60,000</td>
              <td style="text-align: right;">In Transit</td>
              <td style="text-align: right;">Recepient to be determined</td>
            </tr>
          </tbody>
        </table>
      </div>
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