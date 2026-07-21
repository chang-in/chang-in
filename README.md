# 오창인

모바일·웹 서비스를 만들고 직접 운영합니다.

<a href="mailto:dhckddls12@naver.com"><img src="https://img.shields.io/badge/Email-03C75A?style=flat-square&logo=Naver&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white"/></a>

---

## 만든 것

### [fewfew](https://fewfew.app) — 모바일에서 5개 언어 코드 실행·채점
`React Native` `Hono` `Drizzle` · App Store 출시, Android 준비 중 · 1인 개발·운영

iOS의 코드 서명·실행 정책 때문에 런타임 바이너리를 서버에서 내려받아 실행하는 방식은 쓸 수 없었습니다. Python·JavaScript·Java·C·C++ 런타임을 앱에 포함해 실행과 채점을 기기 안에서 처리했습니다. 채점 서버가 필요 없어 오프라인에서도 코드를 컴파일하고 채점할 수 있습니다.

JavaScript 런타임은 QuickJS를 골랐습니다. 빌드 크기와 JIT 없이 실행 가능한지를 기준으로 Hermes·V8과 비교했고, Hermes는 앱 런타임과 사용자 코드의 실행 환경 분리가 어려워, V8은 빌드 크기 증가가 커서 제외했습니다.

API 서버는 Next.js + Prisma 조합이 무거워 더 가벼운 Hono + Drizzle로 옮겼습니다. 전환 전후 기준 Docker 이미지 5배, 메모리 7배 줄었습니다.

### [와이즈픽](https://wise-pick.co.kr) — 건강기능식품 원료·함량 비교
`Next.js` `PostgreSQL` `Prisma` · 1인 개발·운영

제품군마다 비교 기준이 다릅니다(오메가3는 EPA·DHA 함량, 유산균은 균주·CFU). 고정 컬럼 방식은 제품군이 늘 때마다 스키마를 바꿔야 해서 제외하고, 비교 속성을 EAV 구조로 저장했습니다. 조회 복잡도는 늘지만 제품군이 추가돼도 같은 비교 파이프라인에서 처리할 수 있는 쪽을 택했습니다.

식약처 공공데이터에서 1,800여 개 제품의 원료 데이터를 적재했습니다. Cloudflare 캐시 적용 전후 기준으로 주요 조회 응답이 약 1초에서 50ms로 줄었습니다. OCI Always Free 티어에서 운영해 서버 비용은 들지 않습니다(도메인 비용 제외).

### [web-chat-downloader](https://github.com/chang-in/web-chat-downloader) — 웹 AI 대화를 로컬로 백업
`TypeScript` `Chrome Extension` · 공개 저장소

Claude·ChatGPT·Gemini의 웹 대화를 로컬 파일로 백업하는 Chrome 확장입니다. 동기화가 조용히 실패하는 경로를 찾아 고치는 데 대부분의 작업이 들어갔습니다.

- 마지막 백업 이후의 대화만 가져오는 증분 동기화
- 요청 제한에 걸리면 대기했다가 이어받기
- 인덱스를 임시 파일에 쓴 뒤 교체해 중간 실패로 인한 손상 방지
- 짧은 페이지를 목록 끝으로 오해해 대화를 놓치던 문제, 목록 10페이지 상한, 탭이 멈추면 동기화가 매달리던 문제 수정

---

## 오픈소스 PR

모두 Open 상태입니다.

- [expo/expo#44793](https://github.com/expo/expo/pull/44793) — `expo-file-system`의 `./next` 서브패스 export 추가
- [stablyai/orca#9160](https://github.com/stablyai/orca/pull/9160) — 폴더 피커용 프로젝트 기본 디렉터리 설정
- [stablyai/orca#8794](https://github.com/stablyai/orca/pull/8794) — 채팅 임포트 스토리지 · 네이티브 메시징 호스트
- [stablyai/orca#8744](https://github.com/stablyai/orca/pull/8744) — ChatGPT/Claude/Gemini 웹 대화 임포트

`orca#8794`, `orca#8744`는 직접 만든 확장(web-chat-downloader)의 기능을 upstream으로 옮긴 것입니다.
