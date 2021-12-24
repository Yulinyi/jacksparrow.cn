---
title: 播放列表
---

<!-- 使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑 -->

<div class="accordion" id="accordionExample">
    {% for i in site.playlist %}
              <!-- <li><a class="about" href="{{ i.url }}">{{ i.text }}</a></li> -->
    <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree-{{ forloop.index }}">
      <button class="accordion-button p-2 collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree-{{forloop.index}}" aria-expanded="false" aria-controls="collapseThree-{{forloop.index}}">
        {{forloop.index}}.{{ i.author }}&nbsp;({{i.menus.size}})
      </button>
    </h2>
    <div id="collapseThree-{{forloop.index}}" class="accordion-collapse collapse" aria-labelledby="headingThree-{{forloop.index}}" data-bs-parent="#accordionExample">
      <div class="accordion-body p-1">
        <ul class="list-group list-group-flush list-group-item-action">
            {% for item in i.menus%}
            <li class="list-group-item list-group-item-action p-1"><i class="fas fa-play-circle"></i>&nbsp;{{ item }}</li>
            {% endfor %}
        </ul>
      </div>
    </div>
  </div>
  {% endfor %}
</div>