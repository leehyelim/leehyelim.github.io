---
layout: post
title: "css3 input 요소에 placeholder 색상 변경하기"
author: "hyelim"
tags: "css css3 input placeholder color" 
---

::placeholder 가상 셀렉터를 사용하면 색상을 변경할 수 있다.<br><br>
{% highlight css %}
::-webkit-input-placeholder { /* 크롬 4–56 */
    color: #9e9e9e;
}
:-moz-placeholder { /* 파이어폭스 4–18 */
   color: #9e9e9e;
   opacity:  1;
}
::-moz-placeholder { /* 파이어폭스 19–50 */
   color: #9e9e9e;
   opacity:  1;
}
:-ms-input-placeholder { /* 인터넷 익스플로러 10+ */
   color:  #9e9e9e;
}
::placeholder { /* 파이어폭스 51+, 크롬 57+ */
   color: #9e9e9e;
   opacity:  1;
}
{% endhighlight %}
<br>


각각의 prefix는 따로 적어야 한다. 밑에 처럼 작성하면 안됨.<br><br>
{% highlight css %}
::-webkit-input-placeholder,
:-moz-placeholder,
::-moz-placeholder,
:-ms-input-placeholder { ... } /* 이렇게 하면 안돼요! */
{% endhighlight %}
