# Popup Roguelike HTML Prototype

단일 HTML 검증 프로토타입입니다. Unity 프로젝트와 별도로 동작합니다.

## PC에서 실행

브라우저에서 `index.html`을 직접 열면 실행됩니다.

## 같은 와이파이에서 모바일 테스트

PC와 휴대폰이 같은 와이파이에 있어야 합니다.

1. 이 폴더에서 정적 서버를 실행합니다.

```powershell
cd Prototype_HTML\PopupRoguelike
python -m http.server 8080
```

2. PC의 로컬 IP를 확인합니다.

```powershell
ipconfig
```

3. 휴대폰 브라우저에서 아래 형식으로 접속합니다.

```text
http://PC_IP_ADDRESS:8080/
```

예: `http://192.168.0.12:8080/`

## 외부에서 접속하기

GitHub Pages, Netlify, Vercel 같은 정적 호스팅에 `index.html`을 올리면 외부에서도 접속할 수 있습니다.

GitHub Pages 기준:

1. GitHub 저장소를 만듭니다.
2. `Prototype_HTML/PopupRoguelike/index.html`을 저장소에 올립니다.
3. 저장소 Settings > Pages에서 배포 브랜치와 폴더를 선택합니다.
4. 생성된 Pages URL을 휴대폰 브라우저에서 엽니다.

## 모바일 조작

- 왼쪽 하단 가상 조이스틱: 이동
- 터치 드래그: 팝업 이동
- 오른쪽 하단 긴급 닫기 버튼: 가장 오래된 닫을 수 있는 팝업 제거
- 게임 오버 화면의 재시작 버튼: 런 재시작

## 주의

휴대폰만으로 코드 작업을 계속하는 것은 비효율적입니다. 밖에서는 배포 URL로 플레이 테스트와 메모를 하고, 코드 수정은 노트북이나 원격 개발 환경에서 하는 것을 권장합니다.
