---
layout: post
title:  "google analytics"
subtitle: "What is google analytics?"
date:   2021-12-10 23:56:45
categories: [productivity]
comments: true
---


## Google Analytics 란?
![googleanalytics](/img/googleanalytics.png)
현재 구글 마케팅 플랫폼 브랜드 내의 플랫폼으로서, 웹사이트 트래픽을 추적하고 보고하는 구글이 제공하는 웹 애널리틱스 서비스

## Jekyll에 Google Analytics 추가하기
#### 2-1. Google Analytics 계정 만들기
* [Google Analytics](https://analytics.google.com/analytics/web/)에 접속

    * 구글 계정이 없다면, 먼저 구글 가입부터 진행
  
* 사이트 접속 후 측정 시작 클릭

* 새 계정 이름 입력

* 계정 데이터에 대한 권한 설정 

* 통계 플랫폼 선택 (웹 사이트이기 때문에 웹 선택)

* 속성 설정(속성 이름, 보고 시간대, 통화 설정)
##### **중요**
고급 옵션 보기에서 '유니버설 애널리틱스 속성 만들기' 활성화 그 후 자신의 웹사이트 URL 입력 후, 유니버설 애널리틱스 속성만 만들기 체크 **tracking id** 와 **tracking code** 를 얻기 위함
7. 비즈니스 정보 입력 후 만들기
8. 약관 동의

## 2-2. Jekyll 설정 바꾸기
* _config.yml 파일을 열어 Tracking ID 입력
   <br/>`google-analytics: [tracking-id]

* _includes 디렉토리 하위에 google-analytics.html 파일을 생성하고 제공받은 Tracking Code를 복사하고, Tracking Code 중에서 Tracking ID가 할당된 부분은 위에서 선언한 환경 변수로 바인딩해준다.
```html
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-215560049-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'UA-215560049-1');
</script>
```

* 완료
  * 모든 설정이 완료되었다면, Google Analytics 를 통해 실시간으로 활성 사용자가 변하는 것을 볼 수 있다.

