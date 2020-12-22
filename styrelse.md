---
layout: default
title: "Styrelse"
---
# Styrelse
Bostadsrättsföreningens styrelse ska bestå av minst tre ledamöter. Styrelsen utses av föreningsstämman.

{% for item in site.data.board %}
<div class="row">
    <div class="col-sm-3 align-self-center">
        <div class="portraite">
            <img src="assets/img/board/{% if item.img == null %}img-person-placeholder.jpg {% else %}{{item.img}}{% endif %}">
        </div>
    </div>
    <div class="col-sm-6 align-self-center">
        <div class="name">{{ item.name }}</div>
        <div class="desc">{{ item.email }}</div>
        <div class="desc">{{ item.description }}</div>
    </div>
</div>
<hr>

{% endfor %}
