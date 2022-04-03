---
layout: single
author_profile: true
permalink: /music/guitar/
title: "Гитарная музыка"
last_modified_at: 2021-06-04T16:20:02-05:00
custom_css: audioplayer
custom_js: audioplayer
excerpt: "Кликните на трек в списке для начала воспроизведения"
music:
  - name: "Свежий ветер | слова, голос Виталий Митченко | Guitar, Pop"
    url: /assets/audio/04_Fresh_Breeze.mp3
---

[Bits](/music/bits/) | [Поп](/music/pop/) | [Авторские песни](/music/authorsongs/) |
[Баллады](/music/ballads/) | [**Гитарная музыка**](/music/guitar/) | [Фоновая музыка](/music/background/) |

Выберете композицию из списка и нажмите кнопку воспроизведения. Не забудьте нажать на плеере кнопку Unmute! Громкость по умолчанию 30%.

<audio id="audio" preload="metadata" autoplay="false" muted tabindex="0" controls type="audio/mp3">
  <source type="audio/mp3" src="">
  Sorry, your browser does not support HTML5 audio.
</audio>
<ul id="playlist">
  {% for track in page.music %}
    <li>
      <a href="{{ track.url }}"><span class="fas fa-play-circle fa-sm" aria-hidden="true">  {{ track.name }}</span></a>
    </li>
  {% endfor %}
</ul>