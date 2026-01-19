# 안녕하세요 인프라 개발자 오창인 입니다. 

저는 AI를 전공하였고,**Django** 프레임워크와 **Next.js** 프레임워크를 이용해 보안도 탄탄한 서비스를 출시 및 운영 중이고, 주 언어는 Python입니다.

## 📫 Contact

- **Email:** dhckddls12@gmail.com
- **Blog:** [kukurubbing.tistory.com](https://kukurubbing.tistory.com)
- **LinkedIn:** [linkedin.com/in/changin](https://www.linkedin.com/in/changin)
- **Notes:** [qwerty12.notion.site](https://qwerty12.notion.site)


## 🛠 나의 장점들
- **기술의 블랙박스를 파고드는 집요함**: 단순히 도구를 사용하는 데 그치지 않고 내부 동작 원리를 파악합니다. Cloudflare 도입 시 Origin IP 노출 방지를 위한 인프라 구조를 직접 설계하여 보안성을 강화했습니다.
- **비즈니스 가치를 창출하는 실행력**: 아이디어를 빠르게 수익화 가능한 서비스로 구현합니다. 데이터 파싱 자동화부터 인프라 구축까지 전 과정을 리드하며 '지속 가능한 서비스'를 만드는 데 집중합니다.

## 🏆 진행한 프로젝트들

### 와이즈픽 - 합리적 소비 분석 플랫폼 - 개발 진행중...

> **[🔗 서비스 바로가기](https://www.wise-pick.co.kr)**

**3-Tier Architecture**(3계층 아키텍처), 지속적 통합, 배포 자동화 구현.

**Tech Stack:** `Django` `Next.js` `PostgreSQL` `Docker Compose` `Nginx`

**핵심 구현 내용:**
- 📊 **1,200+ 개 시험결과 리포트 데이터 DB 파싱 자동화**
- 🔧 **PostgreSQL JSONB 활용으로 검색 속도 최적화**
- 💾 안정적인 서비스 운영을 위한 DB, STATIC, MEDIA 볼륨 부트 볼륨과 분리작업 및 마운트
- Cloudflare 프록시를 활용한 Origin Server IP 은폐 및 레이어 7(L7) 트래픽 필터링으로 안정적인 서비스 환경 구축

**기술적 의사결정:**
- 향후 효율적인 유지보수를 위한 모놀리식 -> 3계층 아키텍처 사용. 
- 정형 DB만으로는 리포트마다 다른 50+ 필드를 관리 불가 → JSONB 하이브리드 스키마 도입
- 비정형 데이터의 검색 성능 문제 → GIN 인덱스 + ORM 쿼리 최적화로 해결
