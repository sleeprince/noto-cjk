# noto-cjk

## 개요
- [노토(noto) 프로젝트](https://github.com/notofonts/noto-cjk)의 otf 파일을 바탕으로 웹 폰트를 배포한다.
- 바탕체(Sans‐serif)과 돋움체(Serif)를 아우르며, 일곱 가지 굵기를 담고 있다.

## 배경
- 웹 환경에서 현대 한국어와 중세 한국어를 한데 쓸 일이 잦아지며, 예와 이제의 한글을 바르게 나타낼 웹 폰트를 마련하고자 했다.
- 이에 구글의 노토 폰트가 **첫가끝** 방식으로 옛 한글을 지원하여 웹 폰트로서 알맞았다.
- 다만, [구글 폰트](https://fonts.google.com/)에서 내려받은 웹 폰트는 자주 쓰이는 유니코드 영역만을 골라 옛 한글을 나타내지 못하므로, [노토(noto) 프로젝트](https://github.com/notofonts/noto-cjk)에서 곧바로 파일을 받아 웹 폰트로 바꾸었다.
- 아울러 <b>영역 특정 글꼴(Region-specific Subset Fonts)</b>이 보다 적은 용량을 가지나 세로 쓰기를 바르게 나타내지 못하는 탓에, <b>언어 특정 글꼴(Language-specific Fonts)</b>을 끌어썼다.
    - 해당 이슈: https://github.com/notofonts/noto-cjk/issues/79

## 사용법
아래의 코드로써 본고딕(바탕체, Noto Sans)과 본명조(돋움체, Noto Serif)를 가져다 쓸 수 있으며, *family-name*는 `Noto Sans CJK-kr`과 `Noto Serif CJK-kr`이다.
- HTML
```
<link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/sleeprince/noto-cjk@main/notoCJKkr.min.css" />
```
- CSS
```
@import url("https://cdn.jsdelivr.net/gh/sleeprince/noto-cjk@main/notoCJKkr.min.css");
```
## 보기
### ✓ 본고딕 Noto Sans CJK kr
![NotoSans](https://github.com/user-attachments/assets/1104cba7-c855-4c58-8db9-0583c9723be2)
### ✓ 본명조 Noto Serif CJK kr
![NotoSerif](https://github.com/user-attachments/assets/8ba3cf32-e81d-47cd-b901-69672e66cc7c)
