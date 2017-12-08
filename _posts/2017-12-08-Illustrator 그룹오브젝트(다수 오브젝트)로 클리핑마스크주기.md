---
layout: post
title: "Illustrator 그룹 오브젝트(다수 오브젝트)로 클리핑마스크주기"
author: "hyelim"
tags: "illustrator 일러스트레이터 clipping mask 컴파운드 패스 compound path" 
---

### 하나의 오브젝트를 그룹 오브젝트(다수 오브젝트)로 클리핑 마스크를 주고 싶을 때
아래그림과 같이 텍스트에 그라데이션을 씌우고 싶을 땐 클리핑 마스크를 사용한다. 
하지만 클리핑마스크는 단일 오브젝트로만 마스크를 씌울수가 있다. 
텍스트를 아웃라인화 시키면 하나의 오브젝트가 아닌 문자하나하나의 다수 오브젝트로 만들어지기 때문에 마스크를 씌울 수 없다.<br>
![Image](https://user-images.githubusercontent.com/34228953/33755625-08d4954c-dc35-11e7-93a3-7a795ec8355e.png)<br>

아래와 같이 따라해보자.<br>
`오브젝트 그룹 해제 후 - object - compound path - make 한 다음 클리핑마스크 적용`<br>
![Image with caption](https://user-images.githubusercontent.com/34228953/33755708-730bc228-dc35-11e7-8af0-8d7522bd3440.png "Image with caption")_object - compound path - make_<br>

성공!<br>
![image](https://user-images.githubusercontent.com/34228953/33755670-468c2850-dc35-11e7-8fad-7d0086614238.png)<br><br>

컴파운드 패스의 개념은 그려진 순서(오브젝트 그리는 순서에 따른 상하개념)을 무시하고 동일 선상으로 바꿔준다라고 이해하면 될 것 같다.
마스크는 맨 위의 오브젝트로 아래 것을 감싼다라는 것을 생각해보면 조금더 쉽게 이해할 수 있을 것이다.
