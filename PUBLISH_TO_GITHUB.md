# GitHub에 저장소 게시하기

이 문서는 로컬 프로젝트를 본인의 GitHub 계정에 게시하는 절차입니다. 이 환경에서는 사용자의 GitHub 계정에 직접 로그인하거나 원격 저장소를 생성하지 않았습니다.

## 방법 A — GitHub 웹사이트 사용

1. GitHub에 로그인합니다.
2. `https://github.com/new` 로 이동합니다.
3. Repository name에 `AI-RedTeam-Lab`을 입력합니다.
4. README, `.gitignore`, License를 웹에서 추가로 생성하지 않습니다. 이 프로젝트에 이미 포함되어 있습니다.
5. 원하는 공개 범위를 선택하고 저장소를 생성합니다.
6. 아래의 방법 B로 로컬 프로젝트를 push하거나, GitHub 웹 업로드 기능을 이용합니다.

## 방법 B — Git + GitHub CLI

### 1. 도구 설치

- Git: https://git-scm.com/downloads
- GitHub CLI: https://cli.github.com/

설치 후 터미널을 새로 열고 확인합니다.

```bash
git --version
gh --version
```

### 2. GitHub 로그인

```bash
gh auth login
```

브라우저 로그인 절차를 완료합니다.

### 3. 프로젝트 폴더에서 저장소 생성 및 게시

먼저 ZIP을 풀고 `AI-RedTeam-Lab` 폴더로 이동합니다.

```bash
cd AI-RedTeam-Lab
git init
git add .
git commit -m "Initial commit: AI Red Team Lab learning repository"
git branch -M main
gh repo create AI-RedTeam-Lab --public --source=. --remote=origin --push
```

비공개 저장소를 원한다면 마지막 명령의 `--public`을 `--private`로 바꿉니다.

이미 GitHub 웹사이트에서 빈 저장소를 생성했다면 `gh repo create` 대신 해당 저장소의 원격 URL을 연결하고 push합니다.

```bash
git remote add origin https://github.com/YOUR_USERNAME/AI-RedTeam-Lab.git
git branch -M main
git push -u origin main
```

`YOUR_USERNAME`은 본인의 GitHub 사용자명으로 바꿉니다. 이미 `origin`이 등록되어 있으면 `git remote -v`로 확인한 뒤 중복 추가하지 않습니다.

## 게시 전 확인

- [ ] `.env`, 비밀번호, API 토큰, SSH 키를 커밋하지 않았는가?
- [ ] 실습 기록에 실제 시스템의 민감 정보가 없는가?
- [ ] 공개 저장소에 게시해도 되는 자료만 포함했는가?
- [ ] 외부 자료의 라이선스와 출처를 확인했는가?
- [ ] 실습 범위 및 윤리 정책을 이해했는가?
