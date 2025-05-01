# GitHub PR 및 Merge 튜토리얼

- 과제 4까지는 CLI에서 진행
- 과제 5부터는 GitHub 웹사이트에서 진행

## 메인 PUSH 권한 설정됨

- `main` 브랜치는 **직접 push 불가**, PR 필수.

## 목표

`main` 브랜치 보호 정책을 준수하며, 기능 개발 → PR 생성 → 코드 리뷰 → Merge까지
의 과정을 실습

---

## GitHub 리포지토리 Clone

과제1. Mai-Nova organization의 `git-flow` 리포지토리 Clone

## 브랜치 생성

과제2. `feature/{이름이니셜}` 브랜치 생성 및 이동

예시: `feature/shchoi`

- `main`에서 최신 코드 기준으로 브랜치 생성

---

## 코드 수정 및 커밋

과제3. `html/index.html` 파일 수정

예시:

```html
<h1>나는 shchoi 입니다</h1>
```

과제4. 커밋 및 푸시

---

## GitHub에서 Pull Request(PR) 생성

과제5. PR 생성

1. GitHub 웹사이트 이동
2. 복사한 브랜치의 `Compare & Pull Request` 버튼 클릭
3. PR 제목 및 내용 작성
   - 예)
     - 제목: `feat: update index.html content`
     - 설명: `html/index.html 파일 수정`
4. Reviewers에 팀원 추가, Assignee는 본인으로 지정

- 추후 template 추가 예정
- copilot reaview 앱 추가해놨는데 신경 안써도 됩니다

---

## 코드 리뷰 및 Merge

과제6. 코드 리뷰 및 Merge

- 리뷰어가 피드백을 남기면 반영 후 `push`
- 모든 리뷰가 완료되면 Merge 버튼 클릭

  - 참고: `Create a merge commit`, `Squash and Merge`, `Rebase and Merge` 차이를
    확인하면 좋음

- 단, 지금은 테스트 중이므로, 리뷰어가 없어도 본인이 Merge 가능
- 실제 프로젝트에서는 1명 이상의 리뷰가 완료돼야 Merge 가능하도록 설정 예정

---

## 브랜치 정리

과제7. 브랜치 정리

- CLI 혹은 GitHub 웹사이트에서 머지한 브랜치 삭제

```bash
git branch -d feature/shchoi
git push origin --delete feature/shchoi
```

- 리모트/로컬 브랜치 삭제

---

## ✅ 주의 사항

- `main`에 직접 push 불가
- 커밋 메시지 팀 컨벤션 정하고 통일
- 기능 단위로 브랜치 관리 및 PR 자주 올리기
