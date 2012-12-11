---
layout: page
title: 首页
tagline: Supporting tagline
---
{% include JB/setup %}

欢迎！

这个博客建于2012年11月底, 使用Jekyll，托管在github上。博客内容主要是我的学习心得，也关注社会生活，或记录或反思，纯属自娱自乐，不保证质量 ;-)

<!-- 以下代码拷贝自 -->
<!-- http://pingmygeek.com/ -->
<!-- https://github.com/pranavk/pranavk.github.com -->
<!-- 包括_include/post-listing.html -->

<br />
<br />

### 近期博客 ###
---
<!--- ALTERNATIVE TO SHOW POSTS
{% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span>  : <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
-->

{% assign posts = site.posts %}
{% assign listing_limit = 3 %}
{% include post-listing.html %}


<script type="text/javascript">

  var _gaq = _gaq || [];
  _gaq.push(['_setAccount', 'UA-36800439-1']);
  _gaq.push(['_trackPageview']);

  (function() {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
  })();

</script>
