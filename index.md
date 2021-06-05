---
layout: single
author_profile: true
permalink: /
title: "Музыка"
last_modified_at: 2021-06-04T16:20:02-05:00
custom_css: audioplayer
custom_js: audioplayer
excerpt: "Кликните на трек в списке для начала воспроизведения"
header:
  overlay_image: /assets/images/default/musicheader.png
  overlay_filter: 0.5
  caption: "Источник: [**Waveformer**](https://www.misha.studio/waveformer/)"  
music:
  - name: "Музыка 1 | эл.гитара, флейта"
    url: /assets/audio/test.mp3
  - name: "Песня 1 | слова И. Иванова"
    url: http://www.archive.org/download/bolero_69/Bolero.mp3
  - name: "Музыка 2 | ак. гитара, романс"
    url: http://www.archive.org/download/bolero_69/Bolero.mp3
  - name: "Песня 2 | слова П. Васечкина"
    url: http://www.archive.org/download/bolero_69/Bolero.mp3
  - name: "Песня с длинным названием и описанием | эл. гитара, бас, барабаны | слова С. Миронов"
    url: http://www.archive.org/download/bolero_69/Bolero.mp3
  - name: "Музыка 3 | пианино, флейта"
    url: http://www.archive.org/download/bolero_69/Bolero.mp3
  - name: "Синий гном | слова и музыка С. Трубкин | ар. Юлий Леонов"
    url: /assets/audio/test.mp3
---

Привет!

Кликните на трек в списке для начала воспроизведения.
Не забудьте нажать на плеере пиктограмму _unmute_, громкость по умолчанию будет 30%. 

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