---
layout: default
---

<p class="alert" markdown="1">
Hey there, and welcome to **Slap Upside the Head**! Check out some of my favourite posts below, or you can browse nearly eight years of content in [the archives]({{'/archives' | relative_url}})!
</p>

{% assign featured_posts = site.posts | where: "featured", true %}
{% for featured_post in featured_posts %}
<div class="post" markdown="1">
# {{ featured_post.title }}
{{ featured_post.content }}
</div>
{% endfor %}

<p class="alert" markdown="1">
Want more? Check out nearly eight years of posts in [the Slap archives]({{'/archives' | relative_url}})!
</p>