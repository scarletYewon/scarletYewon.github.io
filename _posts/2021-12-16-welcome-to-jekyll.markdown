---
layout: post
title:  "MarkDown!"
date:   2021-12-09 02:32:17 +0900
subtitle: "What is MarkDown?"
categories: [design]
comments: true
---
## 마크다운이란?
![markdown](/img/markdown.png)
마크다운(markdown)은 일반 텍스트 기반의 경량 마크업 언어다. 일반 텍스트로 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다.
HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README 파일이나 온라인 게시물 등에 많이 사용된다.

___

## 사용법
<br/>**마크다운 에디터**<br/>
<br/>마크다운 에디터는 메모장이나 아무 에디터나 사용해도 무방합니다. 다만, 미리보기 기능이 존재하는지 여부에따라 사용성에 큰 차이가 나기때문에, 미리보기 기능이 있는 에디터를 사용하시는 걸 추천드립니다. 또한, 웹으로도 미리보기가 가능한 서비스(Make a README)가 제공되니 간단히 활용하기에는 좋습니다. 
저는 Front 개발에 사용하는 VSCode 에 기본으로 내장되어 있는 마크다운 편집/미리보기 기능을 이용하고 있습니다. 
요즘 대부분의 IDE 에서는 기본 or 확장기능으로 미리보기를 제공하니 사용하시는 IDE에 미리보기 방법을 확인하셔서 사용하시면 됩니다.

___

<br/>
## 1.문법(Syntex)


<br/><strong>제목 - title</strong><br/>
#문자를 1-6개 붙여서 제목을 표현할 수 있습니다. <H1>~<H6> 까지를 지원합니다. 또한, HR(Horizontal Rule, 수평선 구분자)과 결합해서 사용할수도 있습니다.
작성예:
{% highlight ruby %}
# H1
## H2
### H3
#### H4
##### H5
###### H6
{% endhighlight %}
글씨크기 : H1>H2>H3>H4>H5>H6

<br/><strong>강조 - Emphasis</strong><br/>
본문에 특정 문자에 서식(볼드, 이텔릭, 밑줄, 취소선)을 적용해 강조할 수 있습니다.
{% highlight ruby %}
// '*','_','~'기호를 이용하며, 서로 중첩해 사용할 수 있다.
*single asterisks 이텔릭체*
_single underscores 이텔릭체_
**double asterisks 볼드체**
__double underscores 볼드체__
***tripple underscores 볼드+이텔릭체***
___tripple underscores 볼드+이텔릭체___
~~cancelline 취소선~~
**~~bold cancelline 볼드+취소선~~**
<u>underline - 밑줄</u>
{% endhighlight %}

<br/><strong>줄바꿈 - Line Breaks</strong><br/>
마크다운 문법에서는 엔터를 입력해도 개행이 되지 않습니다.
(엔터키 2번 입력은 단락을 나누는 의미) ' ' 공백을 2번 입력하고 엔터로 줄바꿈하면 개행처리가 됩니다.
br태그 사용도 가능합니다

<br/><strong>표 - Table</strong><br/>
본문에 테이블을 넣을 수 있습니다.
헤더 셀을 구분할 때 3개 이상의 -(hyphen/dash) 기호가 필요합니다. 
헤더 셀을 구분하면서 :(Colons) 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다. 
가장 좌측과 가장 우측에 있는 |(vertical bar) 기호는 생략 가능합니다.

---

## 장/단점
**1. 장점**

* 문법이 쉽고 직관적이다.

* 지원 가능한 플랫폼과 프로그램이 다양하다.

* 다양한 형태로 변환이 가능하다.

* Text 형식으로 형상관리를 통한 변경이력관리가 용이하다.

* 별도 도구없이 편집가능 하고 텍스트파일로 용량이 적다. (관리가 용이함)

**2. 단점**

* 아직 표준이 없다.

* 그래서 도구/Viewer에 따라 결과물이 상이할 수 있다.
