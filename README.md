# 여행 N빵 정산

여행 경비(자차 주유비·통행료 포함)를 입력하면 최소 송금 횟수로 정산해 주는 웹앱(PWA).
서버 없이 정적 파일만으로 동작하고, 데이터는 각자 기기의 브라우저에 저장됩니다.

## 파일
- `index.html` — 앱 본체
- `manifest.webmanifest` — 홈 화면 설치 정보(이름, 아이콘, 색)
- `sw.js` — 오프라인 지원. 앱을 고친 뒤에는 `VERSION`을 올리세요.
- `icons/` — 앱 아이콘

## 로컬에서 실행
```
python3 -m http.server 8000
```
브라우저에서 http://localhost:8000 을 엽니다. (`file://`로 직접 열면 설치·오프라인 기능이 꺼집니다.)

## 배포
HTTPS 정적 호스팅(GitHub Pages, Netlify, Cloudflare Pages, Vercel)에 폴더째 올리면 됩니다.
