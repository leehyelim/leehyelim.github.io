---
layout: post
title: "footer 배경이 상단으로 올라갈때"
author: "hyelim"
tags: "css css3 overflow hidden 풋터" 
---

퍼블리싱을 하다보면 아래그림과 같이 풋터의 배경이 상단으로 올라갈 때가 종종있다. <br><br>
![Image](http://blogfiles.naver.net/20140205_166/violetfoam_1391573851554RUQcu_JPEG/layout.jpg)<br>

풋터 상단의 div를 싸고 있는 container의 style에 `overflow:hidden;` 속성을 추가해준다.(다른 속성들은 생략함)<br>
{% highlight html %}
<div id="container" style="overflow:hidden;" >
  <div id="visual"></div>
  <div id="left"></div>
  <div id="right></div>
</div> 

<div id="footer"></div>
{% endhighlight %}
이 속성을 가진 div의 컨텐츠는 해당 div박스 공간안에서만 보여지게 하며, 박스의 공간을 확보하므로 풋터의 컨텐츠가 올라가지 않게 된다.
