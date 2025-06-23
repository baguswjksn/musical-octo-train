---
layout: tag
title: Tags
permalink: tag
---

<section class="max-w-3xl mx-auto px-4 py-8">
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <article class="mb-10 border-l-4 border-blue-200 pl-4">
      <h2 id="{{ tag[0] | slugify }}" class="text-2xl font-semibold text-blue-700 mb-2">
        #{{ tag[0] }} <span class="text-gray-500 text-base">({{ tag[1].size }})</span>
      </h2>
      <ul class="space-y-1">
        {% assign sorted_posts = tag[1] | sort: 'title' %}
        {% for post in sorted_posts %}
          <li>
            <a href="{{ site.baseurl }}{{ post.url }}" class="text-lg text-gray-800 hover:text-blue-600 transition duration-150">
              {{ post.title }}
            </a>
          </li>
        {% endfor %}
      </ul>
    </article>
  {% endfor %}
</section>



