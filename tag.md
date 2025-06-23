---
layout: tag
title: Tags
permalink: tag
---
<section class="max-w-2xl mx-auto">
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <div class="mb-8">
      <h2 id="{{ tag[0] | slugify }}" class="text-xl font-bold text-blue-600 mb-2">
        #{{ tag[0] }}
      </h2>
      <ul class="list-disc list-inside space-y-1">
        {% for post in tag[1] %}
          <li>
            <a href="{{ site.baseurl }}{{ post.url }}" class="text-black hover:underline hover:text-blue-500">
              {{ post.title }}
            </a>
          </li>
        {% endfor %}
      </ul>
    </div>
  {% endfor %}
</section>