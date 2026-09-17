# 오창인

<a href="mailto:dhckddls12@naver.com"><img src="https://img.shields.io/badge/Email-03C75A?style=flat-square&logo=Naver&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white"/></a>

---

## 만든 것

### [fewfew](https://fewfew.app) — 폰 안에서 C++까지 컴파일·채점
`React Native` `Hono` `Drizzle` · 1인 개발 · 운영 · App Store 출시, Android 준비 중

코드를 서버로 보내지 않고 5개 언어 런타임을 앱에 넣어 네트워크 없이 동작하는 앱을 제작했습니다

### [리뷰캐스트](https://reviewcast.co.kr) - 리뷰체험단 플랫폼
개발 및 운영 담당

### [와이즈픽](https://wise-pick.co.kr) — 건강기능식품 원료·함량 비교
`Next.js` `PostgreSQL` `Prisma` · 1인 개발·운영

식약처 공공데이터 1,800여 개 제품을 적재하여 제품군마다 비교 기준이 달라 EAV 구조로 설계했습니다.

### [web-chat-downloader](https://github.com/chang-in/web-chat-downloader) — 웹 AI 대화를 로컬로 백업
`TypeScript` `Chrome Extension` · 공개 저장소

Claude·ChatGPT·Gemini 대화를 로컬 파일로 내려받는 Chrome 확장프로그램 오픈소스 입니다.

이 확장의 임포트 기능을 stablyai/orca에 업스트림 제안했으나([#8744](https://github.com/stablyai/orca/pull/8744)) 메인테이너가 방향을 보류해 닫혔습니다.

---

## 오픈소스 기여

**머지됨**

- [expo/expo#44793](https://github.com/expo/expo/pull/44793) — `expo-file-system`의 `./next` 서브패스 export 추가 · 2026.07 · [CHANGELOG 크레딧](https://github.com/expo/expo/blob/main/packages/expo-file-system/CHANGELOG.md)

**머지 대기**

- [thedotmack/claude-mem#3422](https://github.com/thedotmack/claude-mem/pull/3422) — Chroma 임베딩 함수를 설정으로 노출. 기본값이 영어 전용 모델이라 한국어 검색 품질이 떨어지는 문제를 실제 DB로 측정해 고침 (R@1 12% → 34.5%). 메인테이너가 단독 머지 대상으로 분류
- [chroma-core/chroma-mcp#71](https://github.com/chroma-core/chroma-mcp/pull/71) — 위 PR의 짝. chroma-mcp에 다국어 임베딩 함수 추가
- [stablyai/orca#9160](https://github.com/stablyai/orca/pull/9160) — 폴더 피커용 프로젝트 기본 디렉터리 설정. 메인테이너가 직접 리베이스·확장해 이어가는 중
