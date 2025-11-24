## CodTe: 코딩 테스트 스터디 플랫폼

<br>

## 🧑‍💻 규칙

1. 브랜치 전략
- `main`, `dev`는 항상 존재하며, 기능을 개발할 땐 `dev` 브랜치로부터 분기하여 `feat/기능명` 브랜치를 생성합니다.
- 기능 브랜치의 개발이 완료되면 PR을 통해 `dev` 브랜치로 **Squash and Merge** 합니다.
  - 이유: 기능 브랜치에서의 자잘한 커밋(오타 수정 등)을 없애고, dev에는 기능 단위로 깔끔하게 커밋이 쌓이게 하기 위함
- 프로덕션 배포 준비가 되면 `dev` 브랜치에서 PR을 통해 `main` 브랜치로 **Merge Commit**으로 merge 합니다.
  - 이유: 배포 이력을 명확히 남기고 브랜치 간 그래프를 연결하기 위함

2. 브랜치 컨벤션

- 형식: `태그/설명`
- 태그: feat, fix, docs, chore, design, refactor, cicd
- 예시:
  ```bash
  feat/user-auth-signup-login
  fix/web-header-layout-mobile
  ```

3. 커밋 컨벤션

- 형식: `태그: 요약`
- 태그: Init, Feat, Fix, Docs, Chore, Design, Refactor, CI/CD
- 가능한 작은 단위로 커밋하고, 변경 요약/의도/범위를 명확히 기술합니다.
- 예시:
  ```bash
  Feat: 로그인 기능 추가
  (엔터로 한 칸 띄우기)
  - 소셜 로그인 추가 및 서버로부터 JWT 발급 로직 구현
  - ...
  ```
