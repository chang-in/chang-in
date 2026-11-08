# 오창인
### 웹·앱·AI 개발자

AI를 전공하며 웹·모바일 서비스를 기획해서 만들고 운영합니다. TypeScript(Next.js, React Native)와 Python(Django, FastAPI)을 주로 씁니다. 서울에 살고, 재택 계약직·프리랜서·외주 일을 찾고 있습니다.

<a href="https://chang-in.notion.site/resume" target="_blank"><img src="https://img.shields.io/badge/이력서·포트폴리오-000000?style=flat-square&logo=Notion&logoColor=white" alt="이력서·포트폴리오"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white" alt="LinkedIn 프로필"/></a>
<a href="mailto:dhckddls12@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=Gmail&logoColor=white" alt="이메일 보내기"/></a>
<a href="https://nouscraft.co.kr" target="_blank"><img src="https://img.shields.io/badge/외주_사이트-nouscraft.co.kr-555555?style=flat-square" alt="외주 사이트"/></a>

## 📚 프로젝트

### [fewfew](https://fewfew.app) — 코딩테스트 학습 앱 · App Store 출시
`React Native` `Expo` `Hono` `Drizzle`
- 5개 언어 런타임을 앱에 내장해 기기 안에서 실행·채점
- LLM 문제 생성: 같은 요청은 한 번만 처리하고 하루 호출 예산을 원자적으로 예약, 만든 문제는 검증한 뒤 노출

### [리뷰캐스트](https://reviewcast.co.kr) — 체험단 운영 플랫폼
`Next.js` `PostgreSQL` `Drizzle`
- 두 담당자가 같은 캠페인을 동시에 확정해도 한 번만 처리되도록 트랜잭션과 행 잠금 적용
- 카카오 알림톡 실패 건 재발송, 배포 뒤 버전·로그인을 확인하고 어긋나면 직전 버전으로 자동 복귀

### [와이즈픽](https://wise-pick.co.kr) — 건강기능식품 원료·함량 비교
`Next.js` `PostgreSQL` `Prisma`
- 식약처 공공데이터 1,800여 개 제품 수집·정제, CDN 캐시로 주요 조회 응답 약 1초 → 50ms

> 위 세 서비스는 실제 사용자가 있어 코드는 비공개입니다. 설계와 구현 과정은 [포트폴리오](https://chang-in.notion.site/resume)에 정리했습니다.

### VespaGuard — 말벌 음향 탐지·경보 · 학교 캡스톤(팀장)
`PyTorch` `ONNX Runtime` `ESP32-S3` · 제주한라 AIoT 크리에이터 경진대회 1위
- 다른 녹음 장치에서 탐지율 95%, 꿀벌 오경보 0건. ESP32-S3용 INT8 모델(30KB)

### [web-chat-downloader](https://github.com/chang-in/web-chat-downloader) — 웹 AI 대화를 로컬로 가져오는 Chrome 확장
`TypeScript` `Chrome Extension` · claude.ai·ChatGPT·Gemini 대화를 로컬 세션 파일로 옮겨 터미널에서 이어서 대화

### [nojeom-map](https://github.com/chang-in/nojeom-map) — 길거리 노점 제보·지도 · [데모](https://nojeom-map.vercel.app)
`Next.js` `Leaflet` `PostgreSQL` · 노점 보호를 위해 좌표는 흐려서 보여줌

## 🔥 오픈소스 기여

**머지됨**

- [expo/expo#44793](https://github.com/expo/expo/pull/44793) — `expo-file-system`의 `./next` 서브패스 export 추가 · 2026.07 · [CHANGELOG 크레딧](https://github.com/expo/expo/blob/main/packages/expo-file-system/CHANGELOG.md)
- [thedotmack/claude-mem#3422](https://github.com/thedotmack/claude-mem/pull/3422) — 임베딩 함수를 설정으로 고를 수 있게 해 한국어 검색 개선 · 2026.09. 자체 실험에서 다국어 모델 적용 시 R@1 12% → 34.5%

**진행 중**

- [chroma-core/chroma-mcp#71](https://github.com/chroma-core/chroma-mcp/pull/71) — chroma-mcp에 `multilingual` 임베딩 함수 추가. 위 claude-mem 설정이 이 함수를 고를 수 있게 하는 한 쌍
- [stablyai/orca#9160](https://github.com/stablyai/orca/pull/9160) — 폴더 피커용 프로젝트 기본 디렉터리 설정. 메인테이너가 직접 리베이스·확장해 이어가는 중

<details>
<summary>닫힌 PR 2건</summary>

- [stablyai/orca#8477](https://github.com/stablyai/orca/pull/8477) — AI Vault에 Antigravity 세션 지원 추가 (+1,169/−411). 리뷰 두 차례를 반영하는 사이 메인테이너 구현(#8971)이 먼저 main에 들어가 직접 닫음
- [stablyai/orca#8744](https://github.com/stablyai/orca/pull/8744) — web-chat-downloader의 웹 대화 임포트를 통째로 옮긴 umbrella PR. 메인테이너가 방향을 보류해 닫힘. 1/4로 쪼갠 [#8794](https://github.com/stablyai/orca/pull/8794)도 함께 멈춤

</details>
