---
title: Soapbox Science Tübingen
---

# Speakers

<style type="text/css">
    p {
        text-align: justify;
    }
</style>


<div>
  {% for speaker in site.speakers %}
    <h2 id='{{ speaker.name | slugify: "latin"}}'>{{ speaker.name }}</h2>
    <div>
      <img src="./assets/speakers/{{ speaker.image }}">
    </div>
    {{ speaker.content }}
  {% endfor %}
</div>

