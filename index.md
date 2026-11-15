---
layout: default
---

<div class="home-columns">
  <figure class="home-image">
    <img src="{{ '/assets/hero.png' | relative_url }}" alt="Newscientist Issue 3206 by Tishk Barzanji">
    <figcaption>'Newscientist Issue 3206' by Tishk Barzanji</figcaption>
  </figure>

  <div class="home-text">
    <p>I’m a PhD student in Neurosymbolic AI at TU Graz, working as a part of Bettina Könighofer’s group. My main interest is broadly figuring out how we can formalize normative/ethical rules for artificial systems to follow, and then how to implement them. My prior background is in logic, philosophy, and cognitive science, and still enjoy working on various topics in these fields, including at the intersection of my current one.</p>
    
    <p>I’m also quite interested in helping build better systems for collective alignment. We currently lack the infrastructure to faithfully channel our preferences to parties who hold decision-making power, and to hold them accountable for violations within the system, and I believe this is at the root of many of our contemporary ills. See more in my <a href="{% post_url 2026-07-05-scales-of-alignment %}">white paper</a>.</p>

    <p>At this point, my writings are a bit scattered around all different corners of the web, ranging from denser and technical to airy and conceptual (with some of it previewed on the bottom of this page). See <a href="/research#writing">this</a> little directory where all of them are organized.</p>

  </div>
</div>

<div class="home-writing">
  <h2>Writing</h2>
  <ul class="post-list">
    {% for post in site.posts limit:6 %}
    <li class="post-item">
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
  </ul>
</div>
