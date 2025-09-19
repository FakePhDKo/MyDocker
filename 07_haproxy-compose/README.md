# HAProxy 로드 밸런서 구성 실습 📝
## 📖 프로젝트 개요
이 프로젝트는 HAProxy를 리버스 프록시 및 로드 밸런서로 구성하여, 여러 개의 백엔드 웹 서버에 트래픽을 분산하는 실습입니다. 모든 서비스는 docker-compose.yml 파일 하나로 정의하고, 서비스 확장(--scale) 기능을 활용해 컨테이너화된 애플리케이션의 유연성을 경험했습니다.

# 🚀 주요 학습 내용
+ docker-compose를 이용한 다중 서비스 관리: docker-compose.yml 파일을 통해 여러 컨테이너를 하나의 서비스로 정의하고 실행하는 방법을 배웁니다.

+ HAProxy 설정 파일 관리: 호스트의 haproxy.cfg 파일을 컨테이너에 볼륨 마운트하여 로드 밸런싱 규칙을 적용하는 실무적인 방법을 익힙니다.

+ 서비스 의존성: depends_on을 사용하여 haproxy가 백엔드 web 컨테이너가 시작된 후에 기동되도록 순서를 제어합니다.

+ 수평 확장(Horizontal Scaling): --scale 옵션을 사용해 web 서비스를 여러 컨테이너로 복제하여 트래픽 부하를 분산시키는 방법을 실습합니다.

+ 서비스 디스커버리: haproxy.cfg에서 web 서비스 컨테이너들을 이름으로 찾아 통신하는 Docker Compose의 내장 DNS 원리를 이해합니다.

## 📂 프로젝트 파일 구조
```
.
├── config/
│   └── haproxy.cfg
└── docker-compose.yml
```
+ docker-compose.yml: web 서비스와 haproxy 서비스를 정의하는 파일입니다.

+ config/haproxy.cfg: HAProxy의 로드 밸런싱 규칙을 정의하는 설정 파일입니다.

## 🛠️ 실행 방법
프로젝트 디렉터리로 이동하여 haproxy.cfg 파일과 docker-compose.yml 파일을 확인합니다.

아래 명령어를 통해 web 서비스 컨테이너 3개를 수평 확장하여 실행합니다.

Bash
```bash
docker compose up -d --scale web=3
```
웹 브라우저에서 http://localhost에 접속하여 요청이 세 컨테이너에 분산되는 것을 확인합니다.

실습을 마친 후 아래 명령어로 모든 컨테이너와 리소스를 삭제합니다.

Bash

docker compose down -v
