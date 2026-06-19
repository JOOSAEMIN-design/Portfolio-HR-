# 주세민 포트폴리오 웹사이트

> "숫자로 증명하고, 사람으로 완성하는 HR" — JOO SAEMIN Portfolio

## 📁 파일 구성

```
portfolio/
├── index.html    # 포트폴리오 본문 (단일 파일, 즉시 사용 가능)
└── README.md     # 이 문서
```

## 🚀 사용 방법

### 1) 바로 열어보기
- `index.html`을 더블클릭하면 브라우저에서 바로 열립니다.
- 외부 리소스(Pretendard 폰트, Google Fonts)는 CDN으로 자동 로드됩니다.
- 인터넷 연결이 있는 환경에서 가장 잘 보입니다.

### 2) 무료 호스팅으로 배포하기
어디서나 링크 하나로 공유하고 싶다면, 아래 무료 서비스를 추천합니다.

| 서비스 | 방법 | 결과 URL 예시 |
|---|---|---|
| **Netlify Drop** | https://app.netlify.com/drop 에 `portfolio` 폴더 드래그&드롭 | `https://xxx.netlify.app` |
| **Vercel** | https://vercel.com → New Project → 폴더 업로드 | `https://xxx.vercel.app` |
| **GitHub Pages** | GitHub 리포 생성 → 파일 업로드 → Settings → Pages 활성화 | `https://username.github.io/repo` |
| **Cloudflare Pages** | https://pages.cloudflare.com → Direct Upload | `https://xxx.pages.dev` |

> 💡 가장 빠른 방법: **Netlify Drop**. 회원가입 없이 30초 만에 배포 가능합니다.

### 3) 도메인 연결 (선택)
- 가비아, Namecheap 등에서 도메인 구매 후
- 위 호스팅 서비스의 "Custom Domain" 메뉴에서 연결
- 예: `saemin-joo.com`

## 🎨 디자인 특징

- **밝은 톤 + 충분한 텍스트 대비** — 본문이 진한 슬레이트(#0f172a)로 어디서나 잘 보임
- **블루→인디고→퍼플 그라데이션 액센트** — 신뢰감 있는 HR 톤
- **프로필 사진 + 플로팅 KPI 태그** — 핵심 성과(108.3%, 4.7/5.0)가 사진 주변에 떠 있는 모던 레이아웃
- **글래스모피즘 네비게이션** — 떠 있는 알약 형태의 최신 트렌드 UI
- **KPI 카운트업 애니메이션** — 스크롤 시 핵심 숫자가 0부터 차오릅니다
- **스크롤 리빌(Reveal)** — 섹션이 부드럽게 등장
- **완전 반응형** — 데스크탑/태블릿/모바일 모두 최적화

## ✏️ 직접 수정하는 방법

`index.html`은 단일 파일이라 메모장이나 VS Code로 바로 열어 수정할 수 있습니다.

### 자주 수정할 부분

| 항목 | 위치 (Ctrl+F 검색어) |
|---|---|
| 이름 / 직무 | `JOO SAEMIN`, `HR Recruiter` |
| 메인 카피 | `채용을`, `숫자로 증명하고` |
| KPI 숫자 | `data-count="108.3"` 같은 부분 |
| 회사 / 경력 | `맨파워써치앤컨설팅`, `한솔제지` |
| 자기소개 본문 | `under + stand = understand` 섹션 |
| 연락처 | `seminzzang99@naver.com`, `010-2607-3314` |

### 색상 테마 변경
파일 상단의 `:root` 블록에서 색상을 한 곳에서 바꿀 수 있습니다.

```css
:root {
  --accent:   #2563eb;  /* 메인 블루 */
  --accent-2: #4f46e5;  /* 인디고 */
  --accent-3: #0d9488;  /* 티얼 */
  --text:     #0f172a;  /* 본문 (진한 슬레이트) */
  --text-soft:#475569;  /* 보조 텍스트 */
}
```

### 프로필 사진 교체
HTML 안에서 `<img src="https://www.genspark.ai/api/files/s/FyHLkgX9"` 부분을 찾아 원하는 이미지 URL이나 로컬 경로(`./photo.jpg`)로 바꾸면 됩니다.

## 📞 포함된 정보

- **이름**: 주세민 (JOO SAEMIN)
- **연락처**: 010-2607-3314 · seminzzang99@naver.com
- **위치**: 서울 송파구
- **학력**: 北京外国语大学 (Beijing Foreign Studies University) 정치외교학과
- **경력**:
  - 맨파워써치앤컨설팅 / Talent Delivery Team 인턴 (2025.07–2025.12)
  - 한솔제지 / CDP 2팀 팀장 (2025.04–2025.06)
- **핵심 성과**: 매출 달성률 108.3% · CDP 채택률 60% · 만족도 4.7/5.0

## 📝 라이선스

본 파일은 주세민 개인의 포트폴리오로, 자유롭게 수정·배포하여 사용하실 수 있습니다.

---
Made with care · 2026

## 🖼️ 프로필 사진에 대해

- HTML 파일 안에 사진이 **Base64로 직접 내장**되어 있습니다 → 외부 링크 없이 어디서나 작동
- 별도 파일로도 `profile.jpg`(62KB, 800×1000)를 포함했습니다
- 다른 사진으로 교체하려면:
  1. **간단한 방법**: `profile.jpg`를 새 사진으로 교체하고, HTML의 `<img src="data:image/jpeg;base64,...">` 부분을 `<img src="./profile.jpg">`로 바꾸기
  2. **권장 방법**: 새 사진을 https://www.base64-image.de/ 같은 사이트에서 Base64로 변환 후 src 교체
