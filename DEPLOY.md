# GitHub Pages 배포 가이드

## 1단계: GitHub 저장소 생성

1. [GitHub.com](https://github.com)에 로그인
2. 우측 상단의 **+** 버튼 클릭 → **New repository** 선택
3. 저장소 설정:
   - **Repository name**: `valentine-date` (원하는 이름으로 변경 가능)
   - **Description**: "로맨틱한 발렌타인 데이트 신청 웹앱"
   - **Public** 선택 (GitHub Pages는 Public 저장소에서 무료)
   - **Add a README file** 체크 해제 (이미 README.md가 있음)
4. **Create repository** 클릭

## 2단계: 로컬에서 Git 초기화 및 푸시

터미널에서 다음 명령어들을 순서대로 실행하세요:

```bash
# 현재 디렉토리로 이동
cd "/Users/user/Desktop/cursor/발렌타인데이"

# Git 저장소 초기화
git init

# 모든 파일 추가
git add .

# 첫 커밋
git commit -m "Initial commit: 발렌타인 데이트 신청 웹앱"

# GitHub 저장소와 연결 (YOUR_USERNAME을 본인의 GitHub 사용자명으로 변경)
git remote add origin https://github.com/YOUR_USERNAME/valentine-date.git

# main 브랜치로 이름 변경
git branch -M main

# GitHub에 푸시
git push -u origin main
```

## 3단계: GitHub Pages 활성화

1. GitHub 저장소 페이지로 이동
2. 상단 메뉴에서 **Settings** 클릭
3. 왼쪽 사이드바에서 **Pages** 클릭
4. **Source** 섹션에서:
   - **Branch** 선택
   - `main` 브랜치 선택
   - `/ (root)` 폴더 선택
5. **Save** 클릭

## 4단계: 배포 완료!

몇 분 후 다음 URL로 접속 가능합니다:
- `https://YOUR_USERNAME.github.io/valentine-date/`

이 URL을 공유하면 어디서든 접근할 수 있습니다! 🎉

## 업데이트 방법

코드를 수정한 후 다시 배포하려면:

```bash
git add .
git commit -m "Update: 변경사항 설명"
git push
```

GitHub Pages는 자동으로 업데이트됩니다 (몇 분 소요).

## 문제 해결

### 404 에러가 나는 경우
- 저장소 이름이 `YOUR_USERNAME.github.io`와 정확히 일치하는지 확인
- Settings > Pages에서 배포 상태 확인
- 몇 분 더 기다려보기 (배포에 시간이 걸릴 수 있음)

### 파일이 보이지 않는 경우
- `index.html` 파일이 저장소 루트에 있는지 확인
- 파일명이 정확히 `index.html`인지 확인 (대소문자 구분)

