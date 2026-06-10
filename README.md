# Mobile Viewer - 강의용 모바일 화면 뷰어

AI 도구 활용 강의 시 PC/노트북에서 웹사이트를 **모바일 화면처럼** 보여주는 웹 앱입니다.

## 주요 기능

### 📱 모바일 뷰어
- PC 브라우저에서 URL 입력 → 스마트폰 프레임 안에 모바일 크기로 표시
- 수강생이 자기 폰에서 보는 것과 동일한 화면
- 기기 선택: iPhone 14, iPhone SE, Galaxy S24, iPad Mini
- 세로/가로 모드 전환
- AI 도구 즐겨찾기 (Gemini, ChatGPT, Suno, Canva 등)
- iframe 차단 사이트는 모바일 크기 팝업으로 열기

### 🔗 화면 미러링 가이드
- iPhone AirPlay 미러링 방법
- Android Smart View / USB 미러링 방법
- Windows 무선 미러링 프로그램 안내

## 파일 구성
```
From Web to App_py/
├── index.html      ← 메인 앱
├── manifest.json   ← PWA 설정
├── sw.js          ← 서비스 워커
├── README.md
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## 사용법

### 강사 (PC/노트북)
1. 브라우저에서 앱 열기
2. 왼쪽 패널에서 URL 입력 또는 즐겨찾기 클릭
3. 화면 중앙의 폰 프레임에 모바일 화면 표시
4. 프로젝터로 이 화면을 수강생에게 보여주기

### 배포 방법

#### Netlify (가장 쉬움)
1. https://netlify.com 가입
2. "Add new site" → "Deploy manually"
3. 이 폴더 전체를 드래그&드롭
4. 배포 완료!

#### GitHub Pages
1. GitHub 저장소 생성
2. 파일 업로드
3. Settings → Pages → main branch 선택

## 주의사항
- 많은 사이트(Google, ChatGPT 등)가 iframe 삽입을 차단합니다
- 차단된 사이트는 "모바일 크기 팝업" 버튼으로 열 수 있습니다
- 즐겨찾기 데이터는 브라우저 localStorage에 저장됩니다
