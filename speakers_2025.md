---
title: Soapbox Science Tübingen 2025
---

# Speakers

<style type="text/css">
    p {
        text-align: justify;
    }
</style>


<div>
  {% for speaker in site.speakers25 %}
    <h2 id='{{ speaker.name | slugify: "latin"}}'>{{ speaker.name }}</h2>
    <div>
      <img src="./assets/speakers25/{{ speaker.image }}">
    </div>
    {{ speaker.content }}
  {% endfor %}
</div>

