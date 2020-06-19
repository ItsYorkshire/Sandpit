---
layout: post
title:  "My first blog post"
date:   2020-06-19 10:58:44 +0100
categories: myposts

#Categories
heading: I like cupcakes
show_heading: true
cupcakes:
  - chocolate
  - lemon
  - strawberry

#Disqus
comments: true
# other options
---
My first blog post

[//]: ##categories

{% if page.show_heading %}
  <h1>{{ page.heading | upcase | truncate: 8 }}</h1>
{% endif %}
...
<ul>
{% for cupcake in page.cupcakes %}
  <li>{{ cupcake }}</li>
{% endfor %}
</ul>
...

{% include youtube.html youtube_id="lC51CynVHAU" %}



<div id="disqus_thread"></div>
<script>



/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://https-itsyorkshire-github-io-sandpit.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
