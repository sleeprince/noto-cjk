# noto-cjk

## 개요
- [노토(noto) 프로젝트](https://github.com/notofonts/noto-cjk)의 otf 파일을 바탕으로 웹 폰트를 배포한다.
- 바탕체(Sans‐serif)과 돋움체(Serif)를 아우르며, 일곱 가지 굵기를 담고 있다.

## 배경
- 웹 환경에서 현대 한국어와 중세 한국어를 한데 쓸 일이 잦아지며, 예와 이제의 한글을 바르게 나타낼 웹 폰트를 마련하고자 했다.
- 이에 구글의 노토 폰트가 **첫가끝** 방식으로 옛 한글을 지원하여 웹 폰트로서 알맞았다.
- 다만, [구글 폰트](https://fonts.google.com/)에서 내려받은 웹 폰트는 자주 쓰이는 유니코드 영역만을 골라 옛 한글을 나타내지 못하므로, [노토(noto) 프로젝트](https://github.com/notofonts/noto-cjk)에서 곧바로 파일을 받아 웹 폰트로 바꾸었다.
- 아울러 <b>영역 특정 글꼴(Region-specific Subset Fonts)</b> 또는 <b>언어 특정 가변 글꼴(Language-specific Variable Fonts)</b>이 보다 적은 용량을 가지나 세로 쓰기를 바르게 나타내지 못하는 탓에, <b>언어 특정 글꼴(Language-specific Fonts)</b>을 끌어썼다.
    - 해당 이슈: https://github.com/notofonts/noto-cjk/issues/79

## 사용법
- 아래의 코드로써 본고딕(바탕체, Noto Sans)과 본명조(돋움체, Noto Serif)를 가져다 쓸 수 있으며, *family-name*은 `Noto Sans CJK-kr`과 `Noto Serif CJK-kr`이다.
### jsdelivr CDN
※ jsdelivr에서 내려받을 수 있는 한 파일의 한계 용량은 20MB로, `Noto Serif CJKkr`의 경우 모든 oft 파일이 20MB를 초과할 뿐 아니라 `Noto Serif CJKkr-Bold.woff`(*font-weight* = 700) 파일 또한 20MB를 넘으므로, woff2 형식을 지원하지 않는 Internet Explorer에서 사용이 제한된다.
- HTML
```
<link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/sleeprince/noto-cjk@main/notoCJKkr.min.css" />
```
- CSS
```
@import url("https://cdn.jsdelivr.net/gh/sleeprince/noto-cjk@main/notoCJKkr.min.css");
```

### statically CDN
※ statically에서 내려받을 수 있는 한 파일의 한계 용량은 30MB로, 용량이 가장 큰 oft 파일까지 모두 30MB 미만이므로 모든 환경에서 쓸 수 있다.
- HTML
```
<link rel="stylesheet" as="style" crossorigin href="https://cdn.statically.io/gh/sleeprince/noto-cjk/v1.0/notoCJKkr.css" />
```
- CSS
```
@import url('https://cdn.statically.io/gh/sleeprince/noto-cjk/v1.0/notoCJKkr.css');
```
## 보기
### ✔️ 본고딕 Noto Sans CJK kr
![NotoSansCJKkr](https://github.com/user-attachments/assets/fb79c35a-0e80-4197-8317-dad43ad98d2b)
### ✔️ 본명조 Noto Serif CJK kr
![NotoSerifCJKkr](https://github.com/user-attachments/assets/d8084d78-2252-4d9a-991f-877ff7cd778a)
