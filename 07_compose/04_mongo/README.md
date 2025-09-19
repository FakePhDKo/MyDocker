# Docker Compose: MongoDB + UI 연동 실습📝
## 📖 프로젝트 개요
이 실습은 docker-compose.yml 파일을 사용하여 MongoDB와 Mongo Express 컨테이너를 연동하는 방법을 다룹니다. depends_on, networks, environment 옵션을 활용하여 다중 컨테이너 애플리케이션의 의존성과 설정을 관리하는 방법을 학습합니다.

## 🚀 실습 내용
+ 서비스 의존성: depends_on을 사용하여 mongo 컨테이너가 먼저 시작된 후 mongo-express가 시작되도록 의존 관계를 설정합니다.

+ 환경 변수: environment 필드를 사용하여 MongoDB의 사용자명/비밀번호와 Mongo Express의 접속 URL을 전달합니다.

+ 컨테이너 간 통신: docker-compose의 기본 네트워크를 통해 두 컨테이너가 서로를 이름으로 인식하고 통신하는 것을 확인합니다.

+ 웹 UI 접속: 웹 브라우저로 mongo-express에 접속하여 MongoDB가 정상적으로 연동되었는지 확인합니다.

## 📁 파일 구조

Bash

```bash
.
├── docker-compose.yml
└── image-data/
```
