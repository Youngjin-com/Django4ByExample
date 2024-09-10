# 예제로 배우는 Django 4

<img src="https://www.youngjin.com/images/book_cover/9788931474435.jpg" height="350px" style="border: 2px solid grey;">

[예제로 배우는 Django 4(영진닷컴)](https://blog.naver.com/ydot/223324247963)

『예제로 배우는 Django 4』는 블로그, 소셜 웹사이트, 온라인 상점, e-러닝 플랫폼 등 활용도 넘치는 4가지 예제와 함께 Django를 차근차근 배워 본다. 파이썬을 갓 뗀 분에게도 좋고, 이미 Django를 배웠지만 레퍼런스급 예제를 연습하고 다른 기술과 연계하여 나만의 Django 앱을 확장하고자 하는 용도로 읽기에도 좋다.

이 도서는 실습 파트로만 이루어진 완전 실습형 도서로, 처음부터 예제 프로그램을 만들며 Django의 사용법을 자연스럽게 익힐 수 있도록 구성한 도서이다. 다행히 처음 1~3장부터 어려운 예제 프로그램을 만들지는 않고, 간단한 블로그를 만든다. 물론 Django로 만드는 만큼 웹페이지 부분만을 만들지는 않는다. 기본적인 MTV 패턴부터 쿼리셋, 데이터베이스를 이용한 전문 검색 기능과 같이 백엔드의 요소 또한 다룬다.

그 뒷장부터는 본격적으로 다양한 프로그램을 만든다. 온라인 상점, e-러닝 플랫폼과 같은 앞으로의 프로젝트의 기초로 사용하기 좋은 실용성 좋은 예제가 준비되어 있다. 단순히 겉모습만 묘사하는 선에서 배우지 않고, 소셜 웹사이트라면 소셜 인증, 온라인 상점이라면 외부 결제 모듈 사용법, e-러닝 플랫폼이라면 학생 등록 시스템 구현 등 실제 개발 시 알아 두어야 할 중요 관련 기술이나 구현법도 함께 알려준다.

감이 잘 오지 않는다면, 깊게 고민하지 말고 우선 책을 펼쳐 예제를 타이핑해 보기를 바란다. 중간중간 커피 한 모금 곁들이면 더 좋다. 800 페이지 이상의 분량에 걸쳐 4개의 프로젝트를 쉴 새 없이 만들다 보면 어느새 Django가 확실히 손에 익어 있을 것이다.

**저자** 안토니오 멜레  
**역자** 김성원  
**발행일** 2024년 03월 05일   
**크기** 188*257mm   
**쪽수** 856쪽  
**가격** 38,000원  
**ISBN** 9788931474435  

<br>

## 💡안내
코드는 각 장의 번호에 따라 디렉토리로 구성되어 있습니다. 예를 들어, `Chapter02`는 2장의 소스 코드를 포함하고 있습니다. 각 장의 폴더에는 해당 장의 코드를 실행하기 위해 필요한 모든 패키지를 포함한 `requirements.txt` 파일이 있습니다. 이 패키지들은 `pip install -r requirements.txt` 명령어로 설치할 수 있습니다.

<br>

## 💡요구 사항
이 책은 Python 3.10+와 Django 4.1을 필요로 합니다.

<br>

## 💡정오표
- 1장, *그림 1.4*에서 `body` 필드는 `ForeignKey` 대신 `TextField`여야 합니다.
- 16장, 647쪽의 `ASGI_APPLICATION = 'educa.routing.application'`은 `ASGI_APPLICATION = 'educa.asgi.application'`으로 수정되어야 합니다.

<br>

## 💡Django 프로젝트

이 책에서는 네 가지 Django 프로젝트로 나누어진 다양한 웹 애플리케이션 개발 주제를 다룹니다:

- **블로그 애플리케이션** (1~3장): 완전한 블로그 애플리케이션 만들기
  - 데이터 모델, 뷰, URL 생성
  - 블로그 관리 사이트 구현
  - 모델에 대한 표준 URL 사용 및 게시물에 대한 SEO 친화적인 URL 구현
  - 게시물 페이지네이션 구축 및 클래스 기반 뷰 생성 학습
  - 폼을 사용해 독자가 이메일로 게시물을 공유할 수 있도록 하고 모델 폼을 사용한 댓글 시스템 구현
  - [django-taggit](https://github.com/jazzband/django-taggit)을 사용해 게시물에 태그 추가 및 공유 태그 기반 유사 게시물 추천
  - 최신 게시물 및 댓글이 많은 게시물을 표시하는 커스텀 템플릿 태그 구현
  - [Markdown](https://github.com/Python-Markdown/markdown)을 렌더링하는 커스텀 템플릿 필터 구현
  - 블로그를 위한 사이트맵 및 RSS 피드 생성
  - PostgreSQL을 사용한 전체 텍스트 검색 엔진 구현

- **소셜 웹사이트** (4~7장): 이미지를 북마크하고 공유하는 웹사이트 만들기
  - Django 인증 프레임워크를 사용한 인증 구현
  - 사용자 모델을 커스텀 프로필 모델로 확장
  - Django 메시지 프레임워크 사용
  - 커스텀 인증 백엔드 구축
  - [Python Social Auth](https://github.com/python-social-auth/social-app-django)를 사용해 Facebook, Twitter, Google을 통한 소셜 인증(OAuth2) 구현
  - [django-extensions](https://github.com/django-extensions/django-extensions)를 사용해 HTTPS를 통한 개발 서버 실행
  - [easy-thumbnails](https://github.com/SmileyChris/easy-thumbnails)를 사용해 이미지 썸네일 생성
  - 모델에서 다대다 관계 구현
  - JavaScript와 Django로 북마크릿 구축
  - JavaScript Fetch API와 Django를 사용한 비동기 HTTP 요청 추가
  - 무한 스크롤 페이지네이션 구현
  - 사용자 팔로우 시스템 구축
  - 사용자 활동 스트림 생성 및 QuerySet 최적화
  - Django 신호(signals) 사용법 학습
  - [django-debug-toolbar](https://github.com/jazzband/django-debug-toolbar)를 사용해 디버그 정보 확인
  - [Redis](https://redis.io/)를 사용해 이미지 조회수 카운트
  - Redis로 이미지 순위 시스템 구축

- **전자상거래 애플리케이션** (8~11장): 완전한 기능의 온라인 쇼핑몰 구축
  - 제품 카탈로그 모델 구축
  - Django 세션을 사용한 쇼핑 카트 생성
  - 커스텀 컨텍스트 프로세서 생성
  - 고객 주문 관리
  - [Celery](https://docs.celeryq.dev/)와 [RabbitMQ](https://www.rabbitmq.com/)를 사용한 비동기 알림 전송
  - [Flower](https://github.com/mher/flower)를 사용해 Celery 모니터링
  - [Stripe](https://stripe.com/)와 통합해 결제 처리
  - Stripe의 결제 알림을 수신하기 위한 웹훅 구현
  - Django 관리 사이트에서 커스텀 뷰 생성
  - 관리자 작업(admin actions) 생성 및 CSV 파일 생성
  - [Weasyprint](https://weasyprint.org/)을 사용해 동적으로 PDF 인보이스 생성
  - 주문에 할인 적용을 위한 쿠폰 시스템 구현
  - Stripe 결제와 할인 통합
  - Redis를 사용한 제품 추천 엔진 구축
  - 쇼핑몰에 국제화 적용
  - 번역 파일 생성 및 관리
  - [Rosetta](https://github.com/mbi/django-rosetta)를 사용해 번역 관리
  - URL 패턴 번역 및 언어 선택기 생성
  - [django-parler](https://github.com/django-parler/django-parler)를 사용해 모델 번역
  - [django-localflavor](https://github.com/django/django-localflavor)를 사용해 폼 현지화

- **e러닝 플랫폼** (12~17장): CMS를 포함한 e러닝 플랫폼 구축
  - 강의 모델 생성
  - 데이터 픽스처 사용
  - 모델 상속을 사용해 다형성 콘텐츠 생성
  - 강의 콘텐츠를 정렬하기 위한 커스텀 모델 필드 구현
  - 인증 뷰 구현
  - 클래스 기반 뷰와 믹스인을 사용해 콘텐츠 관리 시스템 구축
  - 그룹과 권한을 사용해 접근 제한
  - 폼세트를 사용해 강의 콘텐츠 관리
  - JavaScript와 Django를 사용해 콘텐츠를 인라인에서 드래그 앤 드롭하여 재정렬 기능 구현
  - [django-braces](https://github.com/brack3t/django-braces)에서 제공하는 제네릭 믹스인 사용
  - 공개 뷰 및 학생 등록 뷰 구현
  - 다양한 유형의 콘텐츠 렌더링 및 [django-embed-video](https://github.com/jazzband/django-embed-video) 사용
  - 캐시 프레임워크를 사용해 콘텐츠 캐시
  - [Memcached](https://memcached.org/) 및 Redis 캐시 백엔드 사용
  - [django-redisboard](https://github.com/ionelmc/django-redisboard)를 사용해 Redis 모니터링
  - [Django REST Framework](https://www.django-rest-framework.org/)을 사용해 API 구축
  - 모델을 위한 시리얼라이저 생성 및 커스텀 API 뷰 생성
  - API 인증 및 권한 처리
  - API 뷰셋 및 라우터 구축
  - Python [requests](https://github.com/psf/requests)를 사용해 API 소비
  - Django [Channels](https://github.com/django/channels)를 사용해 실시간 채팅 서버 구축
  - Django 및 JavaScript로 WebSocket 소비자/클라이언트 구현
  - Redis를 사용해 채널 레이어 설정
  - 완전히 비동기 WebSocket 구현
  - 여러 환경을 위한 설정 생성
  - PostgreSQL, Redis, [Nginx](https://www.nginx.com/), [uWSGI](https://uwsgi-docs.readthedocs.io/en/latest/) 및 [Daphne](https://github.com/django/daphne)를 포함한 [Docker Compose](https://docs.docker.com/compose/)를 사용해 프로덕션 환경 설정
  - HTTPS를 통해 프로젝트를 안전하게 제공
  - Django 시스템 검사 프레임워크 사용
  - 커스텀 미들웨어 구축
  - 커스텀 관리 명령어 생성

<br>

## 💡중간 단계 코드 스니펫
메인 챕터 디렉토리에는 각 장의 완성된 코드만 포함되어 있습니다. [Snippets](https://github.com/PacktPublishing/Django-4-by-example/tree/main/Snippets) 디렉토리에는 각 장의 특정 단계에서 나타나는 코드 파일이 포함되어 있습니다.

장에 대한 중간 파일이 있는 경우, 각 섹션에 대한 하위 폴더 내 `chXX` 폴더에서 해당 파일들을 찾을 수 있습니다. 특정 파일에 대한 수정이 최종 버전과 일치하는 경우, 해당 파일은 중간 파일 트리에 포함되지 않습니다.

변경된 라인은 주석으로 표시됩니다. 전체 블록이 새로 추가되거나 변경된 경우, 변경된 라인의 끝에 해시태그(#)가 표시됩니다.

`filename_00.py`와 같은 파일명은 편집이 적용되기 전의 자동 생성 파일이며, 이는 정보 제공 목적으로만 존재합니다.

<br>

## 💡실습용 예제 파일 & 소스 코드
도서 실습에 필요한 예제 파일과 소스 코드는 챕터별로 구성하였으며, 깃허브 저장소뿐만 아니라 [영진닷컴 홈페이지](https://www.youngjin.com/reader/pds/pds.asp)에서도 다운로드받을 수 있습니다.  
코드 작성 시에는 코드를 직접 입력하거나, 책에서 제공하는 소스 코드 파일을 사용하세요.

<br>

## 💡문의 및 정오표
- [문의](mailto:Support@youngjin.com)
- [정오표](https://www.youngjin.com/Artyboard/mboard.asp?strBoardID=errata)
