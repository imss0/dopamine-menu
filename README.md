# 작은 도파민 메뉴 🌱

딴짓하기 전에 5분짜리 작은 행동 하나를 고르는 개인용 PWA입니다.

## 파일

- `index.html` — 앱 본체
- `manifest.json` — 홈 화면 설치용 PWA 설정
- `sw.js` — 오프라인 캐시
- `icon-*.png` — 앱 아이콘

## 가장 쉬운 사용법

1. 이 폴더를 HTTPS로 서비스되는 정적 호스팅에 올립니다.
2. iPhone Safari에서 페이지를 엽니다.
3. 공유 버튼 → **홈 화면에 추가**를 누릅니다.
4. 홈 화면의 `도파민 메뉴` 아이콘으로 바로 실행합니다.

GitHub Pages, Netlify, Vercel 등의 정적 호스팅에서 사용할 수 있습니다.

## 로컬 테스트

서비스 워커는 `file://`로 연 HTML에서는 정상 동작하지 않습니다.
간단한 로컬 서버를 사용하세요.

```bash
python3 -m http.server 8000
```

그 다음 `http://localhost:8000`으로 접속합니다.

실제 iPhone 설치 테스트는 HTTPS로 배포한 주소에서 하는 것을 권장합니다.
