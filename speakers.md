---
title: Soapbox Science Tübingen
---

# Speakers

<style type="text/css">
    * {
        text-align: justify;
    }
    .speaker-box img {
      display: block;
      margin-left: auto;
      margin-right: auto;
      height: auto;
    }

    .speaker-box {
      margin-top: 3.0rem;
      margin-bottom: 2.0rem;
    }

    .speaker-bio {
      line-height: 1.55;
      padding-left: 0.6rem;
      padding-right: 0.6rem;
    }

    .speaker-talk-title {
      margin-top: 0.95rem;
      margin-bottom: 0.30rem;
      font-weight: 700;
      font-style: italic;
      font-size: 150%;
    }

    .speaker-talk-description {
      margin-top: 0;
      line-height: 1.55;
      padding-left: 0.6rem;
      padding-right: 0.6rem;
      margin-bottom: 2.0rem;
    }

    .div-title {
      color:#159957;
      font-weight: 700;
      font-style: italic;
    }

    .speaker-details hr {
      background-color:rgb(21 153 87 / 0.25);
      height: 4px;
    }

</style>

<div class="speaker-details-all">
  {% for speaker in site.speakers26 %}
  
    <div class="speaker-details" id='{{ speaker.name | slugify: "latin"}}'>
      <hr />

      <div class="speaker-box">
        <img src="./assets/speakers26/{{ speaker.image }}">
      </div>
      <div class="speaker-talk-title">
        <span class="div-title">
          {% if speaker.language == "english" %}SPEAKER{% else %}SPRECHERIN{% endif %}:
        </span> {{ speaker.name }}
      </div>
      {{ speaker.content }}
    </div>
  {% endfor %}
</div>

