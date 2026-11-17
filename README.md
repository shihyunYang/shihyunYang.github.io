# ⚠️ 지우지 마세요 — UnityBuilder 가 Google 드라이브에 APK 를 올리려면 이 페이지가 꼭 필요합니다

## 왜 만들었나

1. UnityBuilder 는 빌드한 APK 를 **Google 드라이브**에 올려 팀원에게 공유한다.
2. 드라이브에 올리려면 Google 계정으로 로그인해 **업로드 권한(토큰)** 을 받아야 한다. 권한은 `drive.file` 하나만 쓴다 (UnityBuilder 가 만든 파일만 다룸).
3. 그 로그인 창(**OAuth 동의 화면**)을 만들 때 Google 이 **앱 홈페이지**와 **개인정보처리방침** 주소를 요구한다. 둘 다 누구나 열 수 있는 공개 웹 페이지여야 한다.
4. 그래서 이 공개 저장소에 두 페이지를 올려 GitHub Pages 로 공개했다. **이 저장소를 지우거나 비공개로 바꾸면 주소가 죽어서** Google 쪽 앱 설정이 막힐 수 있다.

## 주소 (Google Cloud 콘솔의 OAuth 동의 화면에 넣는 값)

| 항목 | 주소 |
|---|---|
| 앱 홈페이지 | https://shihyunyang.github.io/unitybuilder/ |
| 개인정보처리방침 | https://shihyunyang.github.io/unitybuilder/privacy.html |

넣는 곳: Google Cloud 콘솔 › API 및 서비스 › OAuth 동의 화면 (새 화면에서는 Google 인증 플랫폼 › 브랜딩) › 앱 도메인.
받은 토큰은 UnityBuilder 를 돌리는 Mac 의 `gdrive_token.json` 에만 저장된다.

## 왜 별도 공개 저장소인가

UnityBuilder 코드는 비공개 저장소 `unitybuilder` 에 있다. 이 페이지들도 원래 그 저장소에 있었지만
(2026-11-12), 비공개 저장소는 무료 계정에서 Pages 로 공개할 수 없고 11-17 에 코드를 올리면서 덮어써졌다.
그래서 2026-11-18 에 이 공개 저장소로 옮겼다. 다른 앱도 홈페이지·개인정보처리방침이 필요하면 여기 폴더를 하나 더 만들면 된다.
