# 백엔드 개발자 오창인

AI를 전공했고, Python 생태계에 익숙합니다. 현재 군 복무 중 실제 서비스를 운영하며 성능 최적화와 안정성 개선 경험을 쌓고 있습니다.

<a href="mailto:dhckddls12@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=Gmail&logoColor=white"/></a>
<a href="https://kukurubbing.tistory.com" target="_blank"><img src="https://img.shields.io/badge/Tistory-000000?style=flat-square&logo=Tistory&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white"/></a>
<!-- <a href="https://qwerty12.notion.site" target="_blank"><img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=Notion&logoColor=white"/></a> -->

---

## ✨ 저의 장점들

**실제 서비스 운영 경험**  
와이즈픽(Wise Pick)을 기획부터 배포까지 단독으로 진행하여 현재 운영 중입니다. 1,200개 이상의 제품 시험결과 데이터를 자동화 파싱하여 DB에 적재했고, PostgreSQL JSONB와 GIN 인덱스를 활용해 검색 응답시간을 2.3초에서 0.4초로 단축했습니다.

**안정적인 서비스를 위한 인프라 설계**  
Cloudflare 프록시를 통해 Origin Server IP를 은폐하고 L7 레벨 트래픽 필터링으로 외부 공격을 방어합니다. Docker 기반 컨테이너화와 GitHub Actions CI/CD로 안정적인 배포 환경을 구축했습니다.

**비즈니스를 이해하는 개발**  
개발이 수익으로 이어지는 구조를 이해하고 있습니다. Oracle Cloud의 무료 고성능 자원(ARM 4core/24GB)을 전략적으로 활용하여 초기 인프라 비용 없이 서비스를 시작했고, 향후 AWS/GCP 마이그레이션을 고려한 이식 가능한 아키텍처로 설계했습니다.

**본질을 파고드는 학습 습관**  
도구가 제공하는 기능만 사용하지 않고, 공식 문서와 내부 동작 원리를 이해하려 합니다. Cloudflare 도입 시 Origin IP 노출 방지를 위한 인프라 구조를 직접 설계했고, PostgreSQL JSONB의 내부 인덱싱 메커니즘을 학습하여 최적의 쿼리 전략을 수립했습니다.

---

## 🚀 주요 프로젝트

### 와이즈픽 - 합리적 소비 플랫폼
> **[🔗 wise-pick.co.kr](https://wise-pick.co.kr)** | **[📝 기술 블로그](https://kukurubbing.tistory.com/category/와이즈픽)** (2025.12 ~)

> <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=Django&logoColor=white"/> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=Next.js&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/> <img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=Nginx&logoColor=white"/> <img src="https://img.shields.io/badge/Oracle%20Cloud-F80000?style=flat-square&logo=oracle&logoColor=white"/>

**기술적 구현:**
- PostgreSQL JSONB 하이브리드 스키마로 리포트별 가변 필드 50+ 개 유연하게 관리
- GIN 인덱스 + ORM 쿼리 최적화로 검색 응답시간 2.3초 → 0.4초 단축
- Python 자동화 스크립트로 1,200개 리포트 데이터 파싱 (수작업 대비 추정 80시간 → 2시간)
- Cloudflare L7 필터링 + Nginx 리버스 프록시 2단 보안 체계 구축
- GitHub Actions 기반 테스트 자동화 및 배포 파이프라인

**인프라 설계:**
- 3-Tier Architecture (Client - Server - Database 계층 분리)
- Docker 볼륨 분리로 DB/Static/Media 데이터 영속성 확보
- Oracle Cloud ARM 인스턴스 활용, Docker 기반 이식 가능 구조
