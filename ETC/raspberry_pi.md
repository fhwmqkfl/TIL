# 라즈베리파이
> 회사에서 라즈베리 파이를 사용하는데 오늘 작업을 하게 되어 직접 만져보았다.<br>
실제로 라즈베리 파이가 무엇인지에 대해 한번 정리해 보려한다

<img src="https://blog.dalso.org/wp-content/uploads/2020/04/image-187.png">

## 라즈베이파이란?
영국의 라즈베리 재단에서 만든 신용카드 사이즈의 `초소형 컴퓨터` 이다.<br>
성능은 일반 컴퓨터보다 좋지 않지만 기능은 일반컴퓨터와 동일하다(RAM,CPU가 장착되어있고, USB포트와 HDMI입력, 랜선포트 등이 탑재됨)<br>
일반적으로 라즈베리파이는 리눅스 기반의 라즈비안 os를 SD카드에 저장하여 운영체제를 구동 한다<br>
기타 다른 리눅스나 크롬 OS등도 추천되고있다
---
### 개인적 경험
말그대로 초소형 컴퓨터라는걸 체험해본 기분 👩‍💻 <br>
라즈베리 하나에 모든 기능이 구축되어 있어 키보드, 마우스, hdmi, 랜선 연결로 바로 컴퓨터 한 대가 만들 수 있었다 <br>
* 설치화면도 매우 직관적이라 초보자도 쉽게 운영환경을 설정할 수 있을듯 하다
<img src="https://sergeswin.com/media/posts/1116/responsive/image_002-2xl.png">

* 회사에서 사용한 라즈베리 파이의 스펙은 **RPi 3 모델 B**, OS는 **라즈비안 os**로 진행방법은 아래와 같다
  1. 라즈베리파이 이미지 굽기
  2. 이미지를 SD 카드로 쓰기
  3. 구워진 이미지를 사용하여 초기 설정
  4. 적절한 자리에 배치하기