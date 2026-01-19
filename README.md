# 안녕하세요 개발자 오창인 입니다.

**인공지능**를 전공하였고, 현재 군 복무중 개발한 서비스를 운영 중입니다.

## 📫 Contact

<a href="mailto:dhckddls12@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=Gmail&logoColor=white"/></a>
<a href="https://kukurubbing.tistory.com" target="_blank"><img src="https://img.shields.io/badge/Tistory-000000?style=flat-square&logo=Tistory&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white"/></a>
<a href="https://qwerty12.notion.site" target="_blank"><img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=Notion&logoColor=white"/></a>

## ✨나의 장점들

- **추진력**: 군 복무 중 제한된 환경과 시간 속에서도 아이디어를 실제 서비스로 구현하여 출시하였습니다. 단순히 개발에 그치지 않고 실사용자가 이용하는 제품을 안정적으로 운영하고 있습니다.
- 🔬**파고드는 집요함**: 도구가 제공하는 기능을 넘어 내부 동작 원리를 파악합니다. Cloudflare 도입 시 Origin IP 노출 방지를 위한 인프라 구조를 직접 설계하여 외부 공격으로부터 서비스를 보호한 경험이 있습니다.
- 💸**수익화 하는 개발**: 기술은 수익화와 사용자 도달을 위한 도구임을 이해합니다. 데이터 파싱 자동화부터 비용적인 부분에서 효율적인 클라우드 설계까지, '지속 가능한 서비스'를 만드는 전 과정을 주도합니다.
- 💽 **성능 최적화**: 1,200개 이상의 리포트 데이터를 다루며 PostgreSQL의 JSONB와 GIN 인덱스를 활용해 비정형 데이터 검색 성능을 극대화한 경험이 있습니다.
- ⚽ **운동선수 출신의 끈기와 성실함**: 축구선수 생활을 통해 얻은 강한 체력과 목표를 향한 집념을 개발에 투합합니다. 어려운 기술적 난관 앞에서도 끝까지 포기하지 않고 최선의 해결책을 찾아냅니다.

## 🏆 주요 프로젝트

### 와이즈픽 - 합리적 소비 분석 플랫폼(개발 진행중...)

> **[🔗 와이즈픽(wise.pick)](https://www.wise-pick.co.kr)**

**3-Tier Architecture**(3계층 아키텍처), 지속적 통합, 배포 자동화 구현.

**Tech Stack:** `Django` `Next.js` `PostgreSQL` `Docker Compose` `Nginx`

**핵심 구현 내용:**
- 1,200+ 개 시험결과 리포트 데이터 DB 파싱 자동화
- PostgreSQL JSONB 활용으로 검색 속도 최적화
- 정적인 서비스 운영을 위한 DB, STATIC, MEDIA 볼륨 부트 볼륨과 분리작업 및 마운트
- Cloudflare 프록시를 활용한 Origin Server IP 은폐 및 레이어 7(L7) 트래픽 필터링으로 안정적인 서비스 환경 구축

**기술적 의사결정:**
- 향후 효율적인 유지보수를 위한 모놀리식 → 3계층 아키텍처 사용. 
- 정형 DB만으로는 리포트마다 다른 50+ 필드를 관리 불가 → JSONB 하이브리드 스키마 도입
- 비정형 데이터의 검색 성능 문제 → GIN 인덱스 + ORM 쿼리 최적화로 해결
