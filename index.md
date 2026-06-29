---
title: Soapbox Science Tübingen
---

<style type="text/css">

  .grid_container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center; /* Center items horizontally */
      gap: 3%;                /* Use gap instead of margin for spacing */
      row-gap: 30px;          /* Add this for extra vertical space between rows */
      width: 100%;
      margin-bottom: 75px;
      align-items: center;    
  }

  .speaker_box {
      flex: 1 1 21%;           /* 4 per row: 100% / 4 = 25%, minus gap */
      max-width: 23%;          /* Adjust as needed for spacing */
      box-sizing: border-box;
      object-fit: cover;
      text-align: center;
      margin-left: 0;          /* Remove old margins */
      margin-right: 0;
      position: relative;
  }

  .speaker_box img {
    margin-bottom: 10px; /* Adjust this value as needed */
  }

  .speaker_box:hover img {
    transform: scale(1.1);
    filter: grayscale(100%);
  }
</style>

## Our mission

Soapbox Science is a novel public outreach platform for promoting women and
non-binary scientists and the science they do. Events transform public areas
into an arena for public learning and scientific debate; they follow the format
of London Hyde Park’s Speaker’s Corner, which is historically an arena for
public debate. With Soapbox Science, we want to make sure that everyone has the
opportunity to enjoy, learn from, heckle, question, probe, interact with and be
inspired by some of our leading scientists. No middle man, no PowerPoint slide,
no amphitheatre – just remarkable women and non-binary scientists who are there
to amaze you with their latest discoveries, and to answer the science questions
you have been burning to ask. Or simply hear them talk about what
fascinates them, and why they think they have the most fantastic job in the
world!

11 July 2026
{: style="color:#159957; font-size: 200%; font-weight: bold; text-align: center;"}
Tübingen Holzmarkt
{: style="color:#159957; font-size: 150%; font-weight: bold; text-align: center;"}

![](./assets/logos/soapbox_science_poster.png)

Curious about our event? [Sign up to volunteer](https://forms.gle/wCfucpFjNLd5hV1a7) — we'd love to have you!
{: style="font-size: 90%; color: #666; text-align: center; background-color: rgba(21, 153, 87, 0.05); padding: 6px 18px; border-radius: 6px; display: table; margin: 0 auto;"}

## Speakers

<div class="grid_container">
  {% for speaker in site.speakers26 %}
    <div class="speaker_box">
      <a href='speakers.html#{{ speaker.name | slugify: "latin" }}'>
        <img src="./assets/speakers26/{{ speaker.image }}">
      </a>
      {{ speaker.name }}
    </div>
  {% endfor %}
</div>

## Organising team

<div class="grid_container">
  {% for member in site.team %}
    <div class="speaker_box">
      <img src="./assets/organisers/{{ member.image }}">
      {{ member.name }}
    </div>
  {% endfor %}
</div>

## Previous years

### [July 2025]({{ site.baseurl }}{% link speakers_2025.md %})


## Contact
<div style="display: flex; flex-wrap: wrap; gap: 3%; row-gap: 18px; align-items: center; justify-content: center;">
  <div style="display: flex; align-items: center; justify-content: center; gap: 12px; width: 32%;">
    <img src="./assets/logos/icon_email.jpg" alt="Email" style="height: 44px; width: 44px; object-fit: contain;" />
    <a href="mailto:soapboxscience.tuebingen@gmail.com">soapboxscience.tuebingen@gmail.com</a>
  </div>

  <div style="display: flex; align-items: center; justify-content: center; gap: 12px; width: 32%;">
    <img src="./assets/logos/icon_Instagram.jpg" alt="Instagram" style="height: 44px; width: 44px; object-fit: contain;" />
    <a href="https://www.instagram.com/soapboxscience_tuebingen/?hl=en">Instagram</a>
  </div>
</div>

## Partners & Sponsors

<div style="display: flex; flex-wrap: wrap; width: 100%; align-items: center; justify-content: center;">

 <img src="./assets/logos/logo_imprs.png" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_mpg-kyb.webp" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_uni-tue.png" width="32%" style="object-fit: contain;" />

 <div style="flex-basis: 100%; height: 0;"></div>

 <img src="./assets/logos/logo_ecml.jpg" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_rhetai.png" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_mpg-diversity.jpeg" width="32%" style="object-fit: contain; padding: 6px;" />

</div>
