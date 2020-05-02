---
layout: default
title: b{log}
lang: kn
ref: blog
permalink: /blog_kn
comments: false
---
<!-- Featured Image -->
{% include featured-image.html %}
{% assign posts=site.posts %}
<div class="wrapper">
  <section class="section bg-secondary">
    <div class="container">
      <div class="card-profile row justify-content-center" style="margin-top:-40vh">
          <div class="row display-flex justify-content-center">
            <div class="col-lg-8 mt-5" style="min-height: 80vh;">
              {% include starpost.html %}
            </div> 
            <div class="col-lg-4">
              <div class="row display-flex justify-content-center">
                {% for post in posts limit:2 %}
                  <div class="col-lg-12 mt-5">
                    {% include postbox.html %}
                  </div> 
                {% endfor %}
              </div> 
            </div> 
          </div> 
          <div class="row display-flex justify-content-center">
            {% for post in posts offset:2 %}
              <div class="col-lg-4 mt-5">
                {% include postbox.html %}
              </div> 
            {% endfor %}
          </div>
      </div>
    </div>
  </section>
</div>

{% if site.mailchimp-list %}
<!-- Newsletter -->
{% include newsletter.html %}
{% endif %}