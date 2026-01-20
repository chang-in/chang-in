# 백엔드 개발자 오창인

Python 기반 백엔드 개발자입니다.  
AI를 전공했고, 현재 군 복무 중 실제 서비스를 운영하며 성능 최적화와 안정성 개선 경험을 쌓고 있습니다.

<a href="mailto:dhckddls12@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=Gmail&logoColor=white"/></a>
<a href="https://kukurubbing.tistory.com" target="_blank"><img src="https://img.shields.io/badge/Tistory-000000?style=flat-square&logo=Tistory&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/changin" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=LinkedIn&logoColor=white"/></a>
<!-- <a href="https://qwerty12.notion.site" target="_blank"><img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=Notion&logoColor=white"/></a> -->

---

## ✨ 저의 장점들

**실제 서비스 운영 경험**  
wise.pick을 기획부터 배포까지 단독으로 진행하여 현재 운영 중입니다. 1,200개 이상의 제품 시험결과 데이터를 자동화 파싱하여 DB에 적재했고, PostgreSQL JSONB와 GIN 인덱스를 활용해 검색 응답시간을 2.3초에서 0.4초로 단축했습니다.

**안정적인 서비스를 위한 인프라 설계**  
Cloudflare 프록시를 통해 Origin Server IP를 은폐하고 L7 레벨 트래픽 필터링으로 외부 공격을 방어합니다. Docker 기반 컨테이너화와 GitHub Actions CI/CD로 안정적인 배포 환경을 구축했습니다.

**비즈니스를 이해하는 개발**  
개발이 수익으로 이어지는 구조를 이해하고 있습니다. Oracle Cloud의 무료 고성능 자원(ARM 4core/24GB)을 전략적으로 활용하여 초기 인프라 비용 없이 서비스를 시작했고, 향후 AWS/GCP 마이그레이션을 고려한 이식 가능한 아키텍처로 설계했습니다.

**본질을 파고드는 학습 습관**  
도구가 제공하는 기능만 사용하지 않고, 공식 문서와 내부 동작 원리를 이해하려 합니다. 축구선수 시절 기본기 훈련의 중요성을 체득했고, 이를 개발에서도 적용하여 문제의 근본 원인을 찾아 해결합니다.

---

## 🚀 Projects

### 와이즈픽 - 합리적 소비 플랫폼
> **[🔗 wise-pick.co.kr](https://wise-pick.co.kr)** (25.12 ~)

**Tech Stack:**  
<img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=Django&logoColor=white"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=Next.js&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=Nginx&logoColor=white"/>
<img src="https://img.shields.io/badge/Oracle%20Cloud-F80000?style=flat-square&logo=oracle&logoColor=white"/>

**주요 성과:**
- 1,200개 리포트 데이터 파싱 자동화 (수작업 대비 97% 시간 단축)
- JSONB + GIN 인덱스로 검색 성능 82% 개선
- Cloudflare 프록시로 DDoS 방어 및 Origin IP 보호
- GitHub Actions 기반 자동 배포 파이프라인 구축
