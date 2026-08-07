# algorithm_personal_test

이 저장소에 로컬에서 만든 HTML 파일을 업로드하는 방법을 정리한 README입니다.

## 목적
로컬에서 만든 HTML (예: index.html, assets 폴더 등)을 이 저장소에 올리고 필요하면 GitHub Pages로 배포할 수 있습니다.

## 1) Git(권장)으로 업로드하기
터미널에서 다음을 실행하세요 (예: 업로드할 파일이 있는 디렉토리에서):

```bash
# 저장소가 아직 로컬에 없다면 클론
git clone https://github.com/ajjkk01/algorithm_personal_test.git
cd algorithm_personal_test

# 또는 새로운 로컬 저장소를 초기화하는 경우
# git init
# git remote add origin https://github.com/ajjkk01/algorithm_personal_test.git

# 파일 복사 또는 생성 후
git add .
git commit -m "Add local HTML files"

# 기본 브랜치 이름이 main이 아닌 경우 변경하거나 확인하세요
# 예: git branch -M main

git push -u origin main
```

참고: 저장소의 기본 브랜치가 `main`이 아닐 수 있습니다(`master` 등). GitHub 저장소 페이지에서 기본 브랜치를 확인한 뒤 `git push` 시 해당 브랜치 이름을 사용하세요.

## 2) GitHub 웹 인터페이스로 업로드하기
1. 저장소 페이지로 이동합니다: https://github.com/ajjkk01/algorithm_personal_test
2. `Add file` → `Upload files` 선택
3. 로컬 HTML 파일(들)을 드래그 앤 드롭하거나 파일 선택
4. Commit message 입력 후 `Commit changes` 클릭

## 3) GitHub CLI(gh) 사용
```bash
gh repo clone ajjkk01/algorithm_personal_test
cd algorithm_personal_test
# 로컬 HTML 복사
git add .
git commit -m "Add local HTML files"
git push
```

## 4) GitHub Pages로 배포하기 (HTML을 웹사이트로 공개)
1. 저장소 페이지에서 `Settings` → `Pages`로 이동
2. `Source`에서 배포할 브랜치(예: `main`)와 폴더(`/ (root)` 또는 `/docs`) 선택
3. 저장하면 몇 분 내에 사이트가 공개됩니다. URL 형식은 보통:
   `https://ajjkk01.github.io/algorithm_personal_test/`

index.html이 루트에 있으면 해당 URL로 접속 시 페이지가 표시됩니다.

---

원하시면 업로드할 HTML 파일(또는 .zip)을 여기로 올려주시면 제가 대신 커밋해서 푸시해 드릴게요.