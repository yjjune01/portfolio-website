# 📖 포트폴리오 웹사이트 사용 가이드

박유진님의 Story Content Portfolio 웹사이트입니다.

## 📁 파일 구조

```
portfolio/
├── portfolio.html          # 메인 HTML 파일
├── style.css              # 스타일시트
├── images/                # 이미지 폴더
│   ├── divine-cover.jpg           # Divine 표지 이미지
│   ├── orchid-blue-cover.jpg      # 오키드 블루 표지 이미지
│   ├── balance-cover.jpg          # 잃어버린 밸런스 표지 이미지
│   └── aqua-romance-cover.jpg     # 아쿠아로맨스 커버 이미지
└── README.md              # 이 파일
```

## 🖼️ 이미지 추가 방법

1. **이미지 파일 준비**
   - Divine 표지 → `divine-cover.jpg`로 저장
   - 오키드 블루 표지 → `orchid-blue-cover.jpg`로 저장
   - 잃어버린 밸런스 표지 → `balance-cover.jpg`로 저장
   - 아쿠아로맨스 커버 → `aqua-romance-cover.jpg`로 저장

2. **images 폴더에 복사**
   - 모든 이미지 파일을 `images/` 폴더 안에 넣어주세요
   - 파일 이름이 정확히 일치해야 합니다

3. **권장 이미지 사이즈**
   - 표지 이미지: 300px x 400px 이상
   - JPG 형식 권장
   - 파일 크기는 500KB 이하 권장

## ✏️ 내용 수정 방법

### 1. 연락처 정보 수정

`portfolio.html` 파일에서 다음 부분을 찾아 수정하세요:

```html
<!-- Contact 섹션 -->
<p class="contact-info">your.email@example.com</p>  ← 실제 이메일로 변경
<p class="contact-info">010-XXXX-XXXX</p>           ← 실제 연락처로 변경
```

### 2. 구글 드라이브 링크 확인

이미 실제 링크가 들어가 있습니다:
```html
<a href="https://drive.google.com/drive/folders/1pe0K9l6klzLsFJAE-uWSFS9sRbRJpqeg?usp=drive_link">
```

### 3. 색상 변경 (선택사항)

`style.css` 파일 상단에서 색상 변경 가능:

```css
:root {
    --primary-color: #667eea;      /* 메인 색상 (보라) */
    --secondary-color: #764ba2;    /* 서브 색상 (진한 보라) */
    --accent-color: #4fc3f7;       /* 강조 색상 (하늘색) */
}
```

## 🌐 웹사이트 배포 방법

### 방법 1: GitHub Pages (무료, 권장)

1. **GitHub 계정 생성** (없다면)
   - https://github.com 에서 가입

2. **새 Repository 만들기**
   - Repository 이름: `portfolio` 또는 원하는 이름
   - Public으로 설정

3. **파일 업로드**
   - `portfolio.html`, `style.css`, `images/` 폴더 모두 업로드
   - 또는 GitHub Desktop 사용

4. **Settings → Pages 설정**
   - Source: Deploy from a branch
   - Branch: main (또는 master)
   - Folder: / (root)
   - Save 클릭

5. **접속 URL**
   - `https://[사용자명].github.io/[repository명]/portfolio.html`
   - 예: `https://yourusername.github.io/portfolio/portfolio.html`

6. **portfolio.html을 index.html로 변경** (선택사항)
   - 파일 이름을 `index.html`로 바꾸면
   - `https://[사용자명].github.io/[repository명]/` 로 바로 접속 가능

### 방법 2: Netlify (무료, 더 간단)

1. **Netlify 가입**
   - https://netlify.com 에서 가입

2. **Drag & Drop으로 배포**
   - 모든 파일을 선택해서 Netlify 사이트에 드래그
   - 자동으로 배포됨

3. **접속 URL**
   - `https://random-name-123456.netlify.app` 형식
   - 설정에서 원하는 이름으로 변경 가능

### 방법 3: Vercel (무료)

1. **Vercel 가입**
   - https://vercel.com 에서 가입

2. **Import Project**
   - GitHub repository 연결 또는 파일 직접 업로드

3. **자동 배포**
   - 몇 분 내에 자동으로 배포됨

## 📱 모바일에서 확인

- 모든 디자인은 모바일 반응형으로 제작되었습니다
- 스마트폰, 태블릿에서도 깔끔하게 보입니다

## 🎨 디자인 특징

- **모던한 그라디언트** 헤더
- **카드 기반** 레이아웃
- **부드러운 스크롤** 애니메이션
- **호버 효과** 인터랙션
- **반응형 디자인** (모바일 최적화)
- **프린트 최적화** (출력 시 깔끔)

## 🔧 문제 해결

### 이미지가 안 보여요
- 파일 이름이 정확한지 확인하세요
- 대소문자 구분됩니다 (`Divine.jpg` ≠ `divine.jpg`)
- images 폴더 안에 있는지 확인하세요

### 스타일이 안 먹혀요
- `portfolio.html`과 `style.css`가 같은 폴더에 있는지 확인
- 브라우저 캐시 삭제 후 새로고침 (Ctrl + F5)

### GitHub Pages에서 안 보여요
- Repository가 Public인지 확인
- Settings → Pages에서 제대로 설정했는지 확인
- 5-10분 정도 기다려보세요 (배포 시간)

## 💡 팁

1. **이미지 최적화**
   - https://tinypng.com 에서 이미지 압축 추천
   - 로딩 속도가 빨라집니다

2. **SEO 개선** (선택사항)
   - `portfolio.html`의 `<title>` 태그 수정
   - meta description 추가:
   ```html
   <meta name="description" content="박유진 스토리 기획자 포트폴리오">
   ```

3. **커스텀 도메인** (선택사항)
   - GitHub Pages나 Netlify에서 커스텀 도메인 연결 가능
   - 예: `portfolio.yourname.com`

## 📞 도움이 필요하면

- HTML/CSS 수정 관련: Claude에게 물어보세요!
- GitHub Pages 배포: https://pages.github.com
- Netlify 배포: https://docs.netlify.com

## ✅ 체크리스트

배포 전 확인사항:

- [ ] 이미지 4개 모두 추가했나요?
- [ ] 이메일 주소를 실제 주소로 바꿨나요?
- [ ] 연락처를 실제 번호로 바꿨나요?
- [ ] 모든 파일이 한 폴더에 있나요?
- [ ] 브라우저에서 로컬로 테스트해봤나요?
- [ ] 모바일에서도 확인해봤나요?

모든 체크가 완료되면 배포하세요! 🚀

---

**제작:** Claude AI
**마지막 업데이트:** 2024
