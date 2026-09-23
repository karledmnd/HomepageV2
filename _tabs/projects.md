---
layout: page
title: Projects
icon: fas fa-microchip
order: 2
---

{% assign project_posts = site.posts %}

{% if project_posts.size > 0 %}
  <div id="post-list" class="flex-grow-1 px-xl-1">
    {% for post in project_posts %}
      <article class="card-wrapper card mb-3">
        <a href="{{ post.url | relative_url }}" class="post-preview row g-0 flex-md-row-reverse">
          <div class="col-md-12">
            <div class="card-body d-flex flex-column">
              <h1 class="card-title my-2 my-md-0">{{ post.title }}</h1>
              <div class="card-text content mt-0 mb-3">
                <p>{{ post.description | default: post.content | strip_html | truncatewords: 25 }}</p>
              </div>
              <div class="post-meta flex-grow-1 d-flex align-items-end">
                <div class="me-auto">
                  <i class="far fa-calendar fa-fw me-1"></i>
                  {% include datetime.html date=post.date format="%b %d, %Y" %}
                </div>
              </div>
            </div>
          </div>
        </a>
      </article>
    {% endfor %}
  </div>
{% else %}
  <p class="text-muted">No projects published yet.</p>
{% endif %}