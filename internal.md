---
layout: default
title: Internal Environments
permalink: /internal/
---

<div class="page-header">
    <h1 class="page-title">Internal Environments</h1>
    <p class="page-subtitle">Release, Stage, Trial</p>
</div>

<div class="page__content">

    <div class="group-grid">
        {% for group in site.data.internal.groups %}
        <div class="group-block">
            <h2 class="group-title">{{ group.name }}</h2>
            <div class="tiles">
                {% for tile in group.tiles %}
                <div class="tile">
                    <a href="{{ tile.url }}" target="_blank" rel="noopener noreferrer" title="{{ tile.desc }}">
                        <div class="tile-title">{{ tile.title }}</div>
                    </a>
                </div>
                {% endfor %}
            </div>
        </div>
        {% endfor %}
    </div>

</div>
