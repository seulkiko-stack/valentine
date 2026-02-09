# 발렌타인 데이트 신청 웹앱 💕

로맨틱하고 귀여운 발렌타인 데이트 신청 웹사이트입니다.

## 로컬 테스트 방법

### 방법 1: Python 사용
```bash
cd 발렌타인데이
python3 -m http.server 8000
```
그 후 브라우저에서 `http://localhost:8000` 접속

### 방법 2: Node.js 사용
```bash
npx http-server -p 8000
```

### 모바일에서 테스트하기
1. 컴퓨터와 모바일이 같은 Wi-Fi에 연결되어 있어야 합니다
2. 컴퓨터의 로컬 IP 주소 확인:
   - Mac: `ifconfig | grep "inet "` 또는 `ipconfig getifaddr en0`
   - Windows: `ipconfig` (IPv4 주소 확인)
3. 모바일 브라우저에서 `http://[컴퓨터IP]:8000` 접속

## 배포 방법

### GitHub Pages (추천)
1. GitHub에 저장소 생성
2. 파일 업로드
3. Settings > Pages > Source를 `main` 브랜치로 설정
4. `https://[사용자명].github.io/[저장소명]` 접속

### Netlify
1. [netlify.com](https://netlify.com) 접속
2. `index.html` 파일을 드래그 앤 드롭
3. 자동으로 배포 URL 생성

### Vercel
1. [vercel.com](https://vercel.com) 접속
2. 프로젝트 업로드
3. 자동 배포

## 사용 방법
1. 이름을 입력하고 "링크 만들기" 클릭
2. 완성된 화면에서 "링크 공유하기" 버튼 클릭
3. 링크를 카카오톡, 인스타그램 등으로 공유
4. 받는 사람이 링크를 열면 개인화된 데이트 신청 화면 확인

