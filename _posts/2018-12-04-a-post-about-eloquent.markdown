---
layout: post
title:  "Eloquent - Last Query"
date:   2018-12-04 16:08:46 +0700
categories: 
---
put this at the top of the controller :
{% highlight ruby %}
use DB;
{% endhighlight %}

put this right before the query :
{% highlight ruby %}
DB::enableQueryLog();
{% endhighlight %}

put this right after the query :
{% highlight ruby %}
dd(DB::getQueryLog());
{% endhighlight %}
