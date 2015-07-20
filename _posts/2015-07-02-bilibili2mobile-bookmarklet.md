---
layout: post
title: bilibile2mobile bookmraklet
---

    写了一个 bookmarklet ,
    把电脑版 bilibili 的 URL 转换为手机版，
    适用于不想开 Flash Player 的。

<p>
{% highlight js %}
av_id=/bilibili\.com\/video\/av([0-9]+)\//g.exec(location.href)[1];
if (av_id){
    location.href="http://www.bilibili.com/mobile/video/av"+av_id+".html";
}
{% endhighlight %}  
</p>

    JavaScript 链接:
    
<p>
<a href="javascript:av_id=/bilibili\.com\/video\/av([0-9]+)\//g.exec(location.href)[1];if (av_id){location.href=&quot;http://www.bilibili.com/mobile/video/av&quot;+av_id+&quot;.html&quot;}" >bilibili2mobile</a>
</p>
