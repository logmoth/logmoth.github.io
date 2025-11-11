---
layout: home
title: Home
---

# Welcome to My Space

Hi, I'm Rishi. This is my minimalist corner of the internet where I share my thoughts, projects, and experiences.

## What You'll Find Here

- **Blog**: My writings on technology, life, and everything in between
- **Portfolio**: Projects I've worked on and things I've built
- **About**: A bit more about me and what I do

Feel free to explore and reach out if you'd like to connect!

---

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[View all posts →](/blog)
