# 치이카와 카오스 가챠 · GitHub Pages 배포판

모바일 / PC 공용 정적 웹게임입니다. 기존 사용자 기록은 **각 브라우저 localStorage에만** 저장됩니다.

## 배포
1. GitHub에서 `Chiecawa`라는 **새 공개 저장소**를 만듭니다.
2. ZIP 안의 파일들을 압축 해제하고 저장소 **최상위 경로**로 업로드합니다. `index.html`이 최상위에 있어야 합니다.
3. 저장소의 **Settings → Pages → Build and deployment → Source: Deploy from a branch** 선택.
4. **Branch: main / (root)**를 선택하고 Save.
5. 잠시 후 `https://godujan.github.io/Chiecawa/`에서 확인합니다. 이 주소는 실제 배포 후에만 작동합니다.

## 모바일
브라우저에서 게임 링크 접속 후 홈 화면에 추가하면 앱처럼 열 수 있습니다. 브라우저에 따라 설치 메뉴 이름이 다릅니다.

## 주의
- 웹주소 하나로 게임에 접속할 수 있지만 **데이터는 기기 간 동기화되지 않습니다**.
- HTML에 있는 기존 운영자 비밀번호는 클라이언트 코드에 노출되므로 **실제 운영자 인증이 아닙니다**. 다른 기기의 사용자에게 뽑기권을 지급하려면 서버 데이터베이스와 인증 기능이 필요합니다.
- 일일 제한도 현재는 브라우저 단위이므로 서버 기준 부정행위 방지는 지원하지 않습니다.
- 팬게임으로 사용하더라도 원작 캐릭터 이미지의 저작권과 공개 배포 조건은 별개입니다.

## 배포 설정
GitHub 저장소의 Settings → Pages → Build and deployment → Source를 **GitHub Actions**로 설정하세요. `.github/workflows/deploy.yml`이 main push마다 자동으로 배포합니다.
