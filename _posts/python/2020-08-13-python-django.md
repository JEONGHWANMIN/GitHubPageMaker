---
layout: post
current: post
cover: assets/built/images/python-logo.png
navigation: True
title: python - Django-기초(1)
date: 2020-08-13 02:20:00
tags: [python]
class: post-template
subclass: 'post'
author: JEONGHWANMIN
---
### Django
장고란 서버 역할을 할 수 있는 웹 프레임워크 이다. <br>

장고의 장점 <li>많은 것들이 준비되어 있어서 빠르다.<li>보안이 안전하다.<li>스케일이 다양하다<li>다양한 것들을 만들 수 있다.<br>
#### (1) Django install
ex ) pipenv install django (가상환경에 장고 설치)

#### (2) 장고 프로젝트 설치
ex ) django-admin startproject firstproject

장고는 하나의 프로젝트(서비스) 안에 여러개의 앱(큰 기능)으로 구성된다.
#### (3) 장고 서버 실행 하는법 
ex) cd firstproject -> python manage.py runserver
ls 로 manage.py 가 있는 것을 확인하고, runserver !

<img src="assets/built/images/python-logo.png"/>

### 장고의 흐름 ! 
1 ) 요청을 받은 url을 urls.py가 찾는다. <br>
2 ) urls.py에 연결된 views.py의 함수를 실행한다. <br>
2.5 ) templates 를 응답에 담거나, models.py의 데이터를 응답에 담는다. <br>
3 ) views.py에서 응답을 준다.

#### (4) 장고 앱 생성하는 법
python manage.py startapp firstapp
