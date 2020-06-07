---
title: Events
layout: events.liquid
---

<div class="main-container">
<ul class="event-container">
    {%- for events in collections.events %}
    <li>
    <div class="event-inner">
        <div class="event-details">
            <div class="event-name">{{ events.data.title }}</div>
            <div class="event-date">{{ events.data.date }}</div>
            <div class="event-performers">{{ events.data.performers }}</div>
            <div class="event-venue">{{ events.data.venue }}</div>
            <div class="event-more"><a href="{{ events.url }}">more</a></div>
        </div>
        <a href="{{ events.url }}">
            <img alt="{{ events.data.flyer }}" src="/images/{{
                events.data.flyer }}">
        </a>
    </div>
    </li>
    {%- endfor %}

</ul>
</div>
