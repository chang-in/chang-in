# 오창인

모바일·웹 서비스를 만들고 직접 운영하는 1인 개발자입니다. 지금은 [fewfew](https://fewfew.app)와 [리뷰캐스트](https://reviewcast.co.kr)를 운영하고, 쓰는 도구에서 막힌 걸 고쳐 업스트림에 올립니다.

<a href="mailto:dhckddls12@naver.com"><img src="https://img.shields.io/badge/Email-03C75A?style=flat-square&logo=Naver&logoColor=white" alt="이메일 보내기"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white" alt="LinkedIn 프로필"/></a>

---

## 만든 것

### [fewfew](https://fewfew.app) — 폰에서 푸는 코딩테스트 앱
`React Native` `Hono` `Drizzle` · 1인 개발·운영 · App Store 출시, Android 준비 중

코드를 서버로 보내지 않습니다. Python·C·C++·Java·JavaScript 런타임을 앱에 넣어 인터넷이 끊겨도 실행·채점합니다. 풀면 GitHub에 자동 커밋되고, 25단계 티어로 성장이 숫자로 보입니다.

### [리뷰캐스트](https://reviewcast.co.kr) — 관리형 동네 체험단 플랫폼
`Next.js` `PostgreSQL` `Drizzle` · 개발·운영

블로그 소유권·영수증 검증, 체험 매출 리포트, 표기 문구 검수를 담당자가 대신 돌려 사장님이 재계약하게 만드는 서비스입니다. 회원과 어드민 인증을 완전히 분리하고, 선정 확정 알림은 Transactional Outbox로 DB 테이블이 큐 역할을 합니다. Vercel 프로토타입에서 OCI 자체 서버로 옮겨 운영 중입니다.

### [와이즈픽](https://wise-pick.co.kr) — 건강기능식품 원료·함량 비교
`Next.js` `PostgreSQL` `Prisma` · 1인 개발·운영

식약처 공공데이터 1,800여 개 제품을 적재했습니다. 제품군마다 비교 기준이 달라 EAV 구조로 설계했습니다.

### [web-chat-downloader](https://github.com/chang-in/web-chat-downloader) — 웹 AI 대화를 로컬로 백업
`TypeScript` `Chrome Extension` · 공개 저장소

Claude·ChatGPT·Gemini 대화를 로컬 파일로 내려받는 Chrome 확장입니다. 임포트 기능을 stablyai/orca에 업스트림 제안했으나([#8744](https://github.com/stablyai/orca/pull/8744)) 메인테이너가 방향을 보류해 닫혔습니다.

---

## 오픈소스 기여

2026년 9월 기준입니다.

**머지됨**

- [expo/expo#44793](https://github.com/expo/expo/pull/44793) — `expo-file-system`의 `./next` 서브패스 export 추가 · 2026.07 · [CHANGELOG 크레딧](https://github.com/expo/expo/blob/main/packages/expo-file-system/CHANGELOG.md)

**검토 중**

- [thedotmack/claude-mem#3422](https://github.com/thedotmack/claude-mem/pull/3422) — Chroma 임베딩 함수를 설정으로 노출. 기본값이 영어 전용 모델이라 한국어 검색이 약한 문제를 실제 DB의 한국어 코퍼스(후보 200건, 독립 표본 2회)로 측정해 고침 (R@1 12% → 34.5%). 메인테이너가 단독 머지 대상으로 분류
- [chroma-core/chroma-mcp#71](https://github.com/chroma-core/chroma-mcp/pull/71) — chroma-mcp에 `multilingual` 임베딩 함수 추가. 위 claude-mem 설정이 이 함수를 고를 수 있게 하는 한 쌍
- [stablyai/orca#9160](https://github.com/stablyai/orca/pull/9160) — 폴더 피커용 프로젝트 기본 디렉터리 설정. 메인테이너가 직접 리베이스·확장해 이어가는 중
