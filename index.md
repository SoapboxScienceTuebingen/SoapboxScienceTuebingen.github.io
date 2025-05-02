# Soapbox Science Tübingen

<style type="text/css">

  .grid_container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-gap: 3%;
      width: 100%;
      align-items: center;
      margin-bottom: 75px;
  }

  .speaker_box {
      object-fit: cover;
      text-align: center;
      margin-left: 2%;
      margin-right: 2%;
      position: relative;
  }

  .speaker_text {
    position: absolute; top: 50%; left: -25%;
    font-size: 80%; 
    width: 150%; padding: 10px;
    color: #fff; background: rgba(0, 0, 0, 0.75);
  }

  .speaker_text {
    visibility: none; opacity: 0;
    transition: opacity 0.3s;
    z-index: -1;
  }
  .speaker_box:hover .speaker_text{
    visibility: visible; opacity: 1;
    z-index: 1;
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

26 July 2025
{: style="color:#159957; font-size: 200%; font-weight: bold; text-align: center;"}
Tübingen town centre
{: style="color:#159957; font-size: 150%; font-weight: bold; text-align: center;"}

## Speakers

<div class="grid_container">
  {% for speaker in site.speakers %}
    <div class="speaker_box">
      <img src="./assets/speakers/{{ speaker.image }}">
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

## Speaker call - now closed

We are looking for active researchers from STEMM fields (Science, Technology,
Engineering, Mathematics, and Medicine), including PhD students, postdocs,
professors, and beyond, who:

- Are excited about communicating science in an accessible and engaging way.
- Are passionate about connecting with a diverse audience.
- Identify as a woman or non-binary person.

**When**: 26 July 2025

**Where**: Tübingen town centre

![Soapbox science logo](./assets/logos/soapbox_science_call.png){:style="display:block; margin-left:auto; margin-right:auto"}

## Contact

[soapboxscience.tuebingen@gmail.com](mailto:soapboxscience.tuebingen@gmail.com)

<div style="display: inline-flex; width=100%; align-items: center;">

 <img src="./assets/logos/logo_imprs.png" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_mpg-kyb.webp" width="32%" style="object-fit: contain;" />
 <img src="./assets/logos/logo_uni-tue.png" width="32%" style="object-fit: contain;" />

</div>
