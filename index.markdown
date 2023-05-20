---
layout: default
---

<div class="home"> 

  <div class="recipes xs-px1 xs-mt2">
    <div class="clearfix">
    {% assign sorted = site.recipes | sort:"date" %}
    {% for post in sorted %}

      <div class="sm-col sm-col-6 md-col-6 lg-col-4 xs-px1 xs-mb2">
          <a class="block relative bg-blue" href="{{ post.url | prepend: site.baseurl }}">
            <div class="image ratio bg-cover"{% for image in post.image %} style="background-image:url({{site.baseurl}}/images/{{ image }});"{% endfor %}></div>
            <h1 class="title p2 m0 absolute bold white bottom-0 left-0">{{ post.title }}</h1>
          </a>
      </div>
    {% endfor %}
  </div>
  </div>
  
  <div class="container mt4 mb4">
    <div class="sm-col-6 mx-auto px3 sm-px4">
  <p>This is just my little place on the Internet to post the food I cook and the recipes I like. They are usually sized for one or two people, so don’t expect to see 2kg of meat as an ingredient. You might get the opposite issue with me suggesting to use 40 grams of pasta, or a quarter of a tomato - but I’m sure you’ll manage!</p>
  
  <p>Dariusz</p>
  </div>
  </div>

</div>
