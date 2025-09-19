# Docker Compose 실습 총정리 📝
## 📖 프로젝트 개요
이 디렉터리는 Docker Compose를 사용하여 여러 개의 컨테이너로 구성된 애플리케이션을 효율적으로 관리하는 방법을 다룹니다. 단일 컨테이너를 실행하는 복잡한 docker run 명령을 docker-compose.yml 파일로 변환하는 과정을 통해, Compose 파일의 핵심 문법과 기능을 단계별로 학습합니다.

## 🚀 주요 학습 내용
단일 파일로 복수 컨테이너 관리: docker-compose.yml 파일을 통해 여러 컨테이너를 하나의 서비스로 정의하고 실행하는 방법을 배웁니다.

+ 컨테이너 설정 변환: docker run의 -v 옵션은 volumes로, -p는 ports로, command는 command 필드로 어떻게 매핑되는지 익힙니다.

+ 서비스 의존성: depends_on을 사용하여 컨테이너 간의 시작 순서를 제어하는 방법을 학습합니다.

+ 환경 설정: environment 필드로 컨테이너에 환경 변수를 전달하는 실무적인 방법을 이해합니다.

## 📂 프로젝트 디렉터리
+ 01_nginx/: 볼륨 마운트와 컨테이너 이름을 docker run에서 docker-compose.yml로 변환하는 실습입니다.

+ 02_nginx/: 포트포워딩과 이미지 이름을 docker-compose.yml로 변환하고 Nginx 서버를 기동하는 실습입니다.

+ 03_nginx/: 호스트의 설정 파일을 컨테이너에 마운트하고, 컨테이너 실행 명령어를 command 필드로 지정하는 실습입니다.

+ 04_mongo/: MongoDB와 Mongo Express를 depends_on을 사용해 연동하고, 환경 변수를 설정하는 실무적인 예시입니다.

## 🛠️ 실행 방법
각 프로젝트 디렉터리로 이동하여 docker-compose.yml 파일을 확인하고, 아래 명령어로 모든 서비스를 실행해 볼 수 있습니다.

Bash

```bash
# 서비스 실행 (백그라운드)
docker compose up -d

# 실행 중인 서비스 확인
docker compose ps -a

# 서비스 중지 및 컨테이너/네트워크/볼륨 삭제
docker compose down -v
```
