# 가을, 나를 입다 · 배포 안내

## 구성
- `index.html` : 홍보 페이지
- `img/` : 사진·일러스트
- `og.jpg` : 카톡·당근 링크 미리보기 이미지 (1200×630)

## Vercel 배포 (택1)

### A. 터미널
```bash
cd hanam-walking
npx vercel          # 처음 한 번: 로그인 → 프로젝트 이름 hanam-walking 입력
npx vercel --prod   # 실제 주소로 배포
```

### B. GitHub 연결
1. GitHub에 새 저장소를 만들고 이 폴더 내용을 그대로 올림
2. vercel.com → Add New → Project → 저장소 Import
3. Framework Preset: **Other**, 나머지 기본값 → Deploy

### 가장 쉬운 대안: Netlify Drop
app.netlify.com/drop 에 이 폴더를 끌어다 놓으면 바로 주소가 생깁니다.

## 배포 후 꼭 할 것
1. 실제 주소가 `https://hanam-walking.netlify.app` 이 아니면 `index.html`의
   `og:url`, `og:image` 두 줄의 주소를 실제 주소로 바꾸고 다시 배포
2. 카톡 미리보기가 안 바뀌면 developers.kakao.com → 도구 → 공유 디버거에서 주소 입력 후 캐시 초기화

## 다른 강좌로 재사용
`index.html`에서 ✏️ 표시된 부분만 수정 · 색은 `:root`의 토큰 · 개강일은 맨 아래 `START_DATE`
