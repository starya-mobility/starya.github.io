---
layout: default
title: Gallery
permalink: /gallery
---
<!-- Featured Image -->
{% include featured-image.html %}
<div class="wrapper">
  <section class="section bg-secondary">
    <div class="container">
      <div class="card-profile row justify-content-center" style="margin-top:-40vh">
            {% if site.data.galleryset[0] %}
                {% for item in site.data.galleryset %}
                    {% if item.type == "image" %}
                        <div class="col-lg-4 mt-5 article-container">
                            <div class="card shadow border-0 article-img-holder" style="background-color:whitesmoke !important;">
                                <div class="card-header bg-info" style="height: 15rem; padding: unset; margin: 3px;background-color:transparent !important;">
                                    <div style="position: relative;height: 15rem;min-height: 15rem;width: 100%;overflow: hidden;left: 0 !important;">
                                        <a class="stretched-link text-decoration-none" href="{{ item.url }}" data-lightbox="gallery-set" data-title="{{ item.title }}">
                                            <img src="{{ item.url | replace: 'https://res.cloudinary.com/gowrav/image/upload/', 'https://res.cloudinary.com/gowrav/image/upload/w_300/' }}" style="position: absolute;top: 50%;left: 50%;min-width: 100%; z-index: 0;-ms-transform: translateX(-50%) translateY(-50%);-moz-transform: translateX(-50%) translateY(-50%);-webkit-transform: translateX(-50%) translateY(-50%);transform: translateX(-50%) translateY(-50%);">
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    {% endif %}
                {% endfor %}
            {% endif %}
      </div>
    </div>
  </section>
</div>

<script>
  window.addEventListener('DOMContentLoaded', function() {
      (function($) {
          $('.article-container').mouseover(function() {
              $(this).find('.article-img-holder').css('transform', 'scale(1.08)');
          });
          $('.article-container').mouseout(function() {
              $(this).find('.article-img-holder').css('transform', 'scale(1)');
          });
      })(jQuery);
  });
</script>
