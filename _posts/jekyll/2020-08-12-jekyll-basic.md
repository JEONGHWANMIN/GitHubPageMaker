---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: jekyll - 블로그 연습중 !!
date: 2020-08-10 10:18:00
tags: [jekyll]
class: post-template
subclass: 'post'
author: JEONGHWANMIN
---
까먹을거 같은 명령어 

#### 메뉴 추가 
1._data -> tag수정 <br>2._includes -> navigation.html 수정<br>3. _posts 폴더 추가후 파일에 
태그 바꿔주기

#### 파일내 목차 추가 
1. python-table-of-contents.html 만든다.
ex) 내용예시
~~~html
<span class="table-of-contents-list">Python 강좌는 여러 절로 구성되어 있습니다. </span>
   <ul class="table-of-contents-list">
       <li><a href="./python-basic">Python 강좌(1) - Python 기본</a></li>
       <li><a href="./python-control-statement">Python 강좌(2) - Python 제어문</a></li>
   </ul>
~~~
2. _includes 폴더에 저장해서 관리
3. post 안에 이런식으로 추가해준다.
 ~~~
---
layout: post
current: post
cover:  assets/built/images/python-logo.png
navigation: True
title: Python 강좌(1) - Python 기본 
date: 2018-09-27 16:40:00
tags: [python]
class: post-template
subclass: 'post tag-python'
author: moon9342
---

{% include python-table-of-contents.html %}

~~~

수정

