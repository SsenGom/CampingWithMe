# 불멍캠프

말없이 같이 앉아 불멍하는 온라인 캠핑장. 브라우저에서 바로 열리는 Three.js 단일 페이지입니다.

## 배포 (GitHub Pages)

1. 이 폴더를 GitHub 레포(`main` 브랜치)에 push
2. 레포 **Settings → Pages → Build and deployment → Source** 를 **GitHub Actions** 로 선택
3. **Actions** 탭에서 `Deploy to GitHub Pages` 워크플로가 끝나면 `https://<아이디>.github.io/<레포이름>/` 으로 접속

이후로는 `main`에 push할 때마다 자동으로 다시 배포됩니다.

## 구성

| 파일 | 역할 |
|---|---|
| `index.html` | 게임 전체 (Three.js r128은 CDN에서 로드) |
| `.github/workflows/deploy.yml` | push 시 GitHub Pages 자동 배포 |
| `.nojekyll` | Jekyll 처리 건너뛰기 |

## 조작

- 땅 탭/클릭 또는 WASD로 이동, Shift로 뛰기, 드래그로 시점 회전, 휠로 확대
- 가까이 가면 할 수 있는 행동(장작, 해먹, 텐트, 물수제비, 리본 나무, 버스킹 등)이 하단 버튼으로 표시

## 참고

- 다른 캠퍼는 현재 봇입니다. 실시간 멀티플레이는 별도 서버(예: PartyKit) 연동이 필요합니다.
- 리본·물수제비 기록은 각자 브라우저(localStorage)에만 저장됩니다.
- 버스킹 곡은 저작권이 만료된 곡(퍼블릭 도메인)만 사용합니다.
