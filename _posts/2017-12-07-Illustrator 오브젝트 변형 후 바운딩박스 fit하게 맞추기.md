---
layout: post
title: "Illustrator 오브젝트 변형 후 바운딩박스 fit하게 맞추기"
author: "hyelim"
tags: "illustrator 일러스트레이터 bounding box"
---

오브젝트를 회전하면 바운딩박스가 수평적이지 않고 같이 회전한다. 그럴때는 `Object - Transform - Reset Bounding Box` 를 해주면 해결이 된다.<br><br>
하지만 오브젝트 변형 후(삼각형과 같은 도형 꼭지점을 라운드를 준다던지..) 아래그림과 같이 바운딩 박스가 오브젝트에 딱 맞춰지지 않는 현상이 생긴다.<br>
![image](https://user-images.githubusercontent.com/34228953/33744925-338953b0-dbf7-11e7-82b6-0bd1d6d12169.png)

`effect - path - outline object 한 후 object - expand appearance`

![image with caption](https://user-images.githubusercontent.com/34228953/33744936-448917d6-dbf7-11e7-8f25-53a6fd10a0d8.png "Image with caption")_effect -> path -> outline_<br>

![image with caption](https://user-images.githubusercontent.com/34228953/33744943-4dd9d96a-dbf7-11e7-9d86-ab486046ad2f.png "Image with caption")_object -> expand appearance_<br>

이제 바운딩 박스가 fit하게 맞는다! <br>
![image](https://user-images.githubusercontent.com/34228953/33744947-55d2062e-dbf7-11e7-810a-42f4c5695998.png)

