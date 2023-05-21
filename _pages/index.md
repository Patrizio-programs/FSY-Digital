---
layout: page
title: Home
id: home
permalink: /
---

# Welcome to FSY!

<p style="padding: 3em 1em; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Counselors - Roles, Responsibilities, and Duties]]</span> to get started if you are a counselor.
</p>

<p style="padding: 3em 1em; background:  border-radius: 4px;">
  Likewise for Assistant Coordinators: <span style="font-weight: bold">[[Assistant Coordinators - Roles, Responsibilities, and Duties]]</span>.
</p>

<p style="padding: 3em 1em; border-radius: 4px;">
  And for Coordinators: <span style="font-weight: bold">[[Coordinators - Roles, Responsibilities, and Duties]]</span>.
</p>

<strong>Recently updated notes:</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
