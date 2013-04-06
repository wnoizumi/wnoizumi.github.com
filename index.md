---
layout: page
title: Willian Oizumi
tagline:
---

## About me

I am developing software systems since 2009. Despite having already developed pet web applications, I only worked in companies with desktop systems. 
I am enthusiastic about programming and software architecture. My favorite languages are C# and Ruby,
In 2012 I received my BSc. degree in Computer Science from The State University of Maringa. In this course I participated in a research project about evaluation of software architectures. I'm currently a MSc. student in the Informatics Department at PUC-Rio. I am also a member of the OPUS research group. My advisor is Alessandro Garcia.

##Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
