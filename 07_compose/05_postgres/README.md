# Docker Compose: PostgreSQL & Adminer 연동 실습 🐘
## 📖 프로젝트 개요
이 실습은 docker-compose.yml 파일을 사용하여 PostgreSQL 데이터베이스와 웹 기반 관리 도구인 Adminer를 연동하는 방법을 다룹니다. 데이터베이스와 UI 서비스를 하나의 파일로 정의하고 관리하는 방법을 학습합니다.

## 🚀 주요 학습 내용
+ 서비스 의존성: PostgreSQL 컨테이너가 먼저 시작되도록 의존 관계를 설정합니다.

+ 공유 메모리 설정: PostgreSQL과 같은 DB 컨테이너는 shm_size 설정을 통해 성능을 최적화할 수 있음을 학습합니다.

+ 환경 변수 활용: environment 필드를 사용하여 데이터베이스의 사용자명과 비밀번호를 안전하게 전달합니다.

## 📁 파일 구조
```
.
├── docker-compose.yml
└── ...
```
