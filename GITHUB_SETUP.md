# GitHub 저장소 생성 및 배포 가이드

## ⚠️ 중요: 먼저 GitHub에서 저장소를 생성해야 합니다!

## 1단계: GitHub 저장소 생성

### 방법 1: 웹 브라우저에서 생성 (권장)

1. **GitHub 로그인**
   - https://github.com 에 접속하여 로그인

2. **새 저장소 생성**
   - 우측 상단의 **+** 버튼 클릭
   - **New repository** 선택

3. **저장소 설정**
   - **Repository name**: `lete-skill-simulator` (또는 원하는 이름)
   - **Description**: "레테 스킬 시뮬레이터 웹페이지" (선택사항)
   - **Public** 선택 ⚠️ (GitHub Pages 무료 사용을 위해 필수)
   - **Add a README file** 체크 해제 (이미 README가 있으므로)
   - **Add .gitignore** 체크 해제 (이미 .gitignore가 있으므로)
   - **Choose a license** 선택 안 함

4. **Create repository** 버튼 클릭

5. **저장소 URL 확인**
   - 생성 후 나타나는 페이지에서 URL을 복사
   - 예: `https://github.com/your-username/lete-skill-simulator.git`
   - ⚠️ `your-username`을 본인의 실제 GitHub 사용자명으로 확인!

### 방법 2: GitHub CLI 사용 (선택사항)

```bash
gh repo create lete-skill-simulator --public --source=. --remote=origin --push
```

## 2단계: 로컬 저장소를 GitHub에 연결

저장소를 생성한 후, 다음 명령어를 실행하세요:

```powershell
# 1. 원격 저장소 추가 (URL을 본인의 것으로 변경!)
git remote add origin https://github.com/YOUR-USERNAME/lete-skill-simulator.git

# 2. 기본 브랜치 확인
git branch

# 3. GitHub에 푸시
git push -u origin main
```

⚠️ **주의사항:**
- `YOUR-USERNAME`을 본인의 실제 GitHub 사용자명으로 변경하세요
- 저장소 이름이 다르면 URL의 저장소 이름도 변경하세요

## 3단계: GitHub Pages 활성화

1. GitHub 저장소 페이지로 이동
2. 상단 메뉴에서 **Settings** 탭 클릭
3. 왼쪽 사이드바에서 **Pages** 클릭
4. **Source** 섹션에서:
   - **Branch**: `main` 선택
   - **Folder**: `/ (root)` 선택
5. **Save** 버튼 클릭

## 4단계: 웹사이트 확인

- 몇 분 후 다음 주소로 접속 가능:
  - `https://YOUR-USERNAME.github.io/lete-skill-simulator/`
- 배포 상태는 저장소의 **Settings → Pages**에서 확인 가능
- 초록색 체크 표시가 나타나면 배포 완료!

## 문제 해결

### "Repository not found" 오류가 발생하는 경우:
1. ✅ GitHub에서 저장소를 생성했는지 확인
2. ✅ 저장소 URL이 정확한지 확인 (사용자명, 저장소명)
3. ✅ 저장소가 Public인지 확인
4. ✅ GitHub에 로그인되어 있는지 확인

### 인증 오류가 발생하는 경우:
- Personal Access Token이 필요할 수 있습니다
- GitHub Settings → Developer settings → Personal access tokens에서 생성

## 다음 명령어 (저장소 생성 후 실행)

```powershell
# 저장소 URL 확인 후 실행
cd d:\AutoTool\ECT\SKILL
git remote add origin https://github.com/YOUR-USERNAME/lete-skill-simulator.git
git push -u origin main
```
