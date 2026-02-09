# 새 저장소 생성 및 배포 가이드

## 1단계: GitHub에서 새 저장소 생성

1. [GitHub.com](https://github.com)에 로그인
2. 우측 상단의 **+** 버튼 클릭 → **New repository** 선택
3. 저장소 설정:
   - **Repository name**: `valentine`
   - **Owner**: `idus` 선택 (또는 `idus` 조직이 없다면 본인 계정으로 생성 후 나중에 전송)
   - **Description**: "너에게 할 말이 있어 - 로맨틱한 발렌타인 메시지 웹앱"
   - **Public** 선택
   - **Add a README file** 체크 해제
   - **Add .gitignore** 체크 해제
   - **Choose a license** 선택 안 함
4. **Create repository** 클릭

## 2단계: 로컬에서 원격 저장소 변경 및 푸시

터미널에서 다음 명령어를 실행하세요:

```bash
cd "/Users/user/Desktop/cursor/발렌타인데이"

# 변경사항 커밋
git add .
git commit -m "Update: 문구 변경, OG 이미지 추가, 링크 URL 변경"

# 원격 저장소를 새 저장소로 변경
git remote set-url origin https://github.com/idus/valentine.git

# 새 저장소에 푸시
git push -u origin main
```

## 3단계: GitHub Pages 활성화

1. 새 저장소 페이지로 이동: https://github.com/idus/valentine
2. **Settings** 탭 클릭
3. 왼쪽 사이드바에서 **Pages** 클릭
4. **Source** 섹션:
   - **Branch**: `main` 선택
   - **Folder**: `/ (root)` 선택
5. **Save** 클릭

## 4단계: 배포 완료!

몇 분 후 다음 URL로 접속 가능합니다:
- **https://idus.github.io/valentine/**

## 참고사항

- `idus` 조직이 없다면:
  - 본인 계정으로 저장소를 생성하거나
  - GitHub에서 `idus` 조직을 먼저 생성해야 합니다
  - 또는 저장소 이름을 `valentine`으로만 생성하고 URL은 `https://[본인계정].github.io/valentine/`이 됩니다

