# Flask & Redis 애플리케이션 구축 실습 📝
## 📖 프로젝트 개요
이 프로젝트는 Docker Compose를 사용하여 간단한 Flask 웹 애플리케이션과 Redis 데이터베이스를 연동하는 실습입니다. 애플리케이션은 Redis를 이용해 페이지 방문 횟수를 기록하며, docker-compose를 통해 두 개의 컨테이너를 효율적으로 관리하는 방법을 배웁니다.

## 🚀 주요 학습 내용
+ docker-compose.yml 파일을 이용해 web (Flask)과 redis 서비스를 정의하고 연결했습니다.

+ 개발 편의성을 위해 바인드 마운트 볼륨을 사용하여, 소스 코드 수정 시 즉시 컨테이너에 반영되는 핫 리로딩(hot-reloading)을 구현했습니다.

+ docker compose up -d, docker compose down, docker compose run 등 다양한 명령어를 사용해 컨테이너의 생명주기를 제어하는 방법을 익혔습니다.

+ app.py에서 host='redis'처럼 서비스 이름을 사용해 컨테이너 간에 통신하는 서비스 디스커버리 원리를 확인했습니다.

## 📂 프로젝트 파일 구조
+ app.py: Flask 웹 애플리케이션 소스 코드.

+ requirements.txt: Flask와 Redis 패키지 목록.

+ Dockerfile: Flask 앱 이미지를 빌드하기 위한 파일.

+ docker-compose.yml: web과 redis 서비스를 정의하는 파일.

## 🛠️ 실행 방법
+ 07_composetest 디렉터리로 이동합니다.

+ docker compose up 명령어로 컨테이너들을 기동합니다.

Bash

```bash
docker compose up
```
웹 브라우저에서 http://localhost:8000에 접속하여 페이지 방문 횟수가 증가하는 것을 확인합니다.

실습을 마친 후 아래 명령어로 모든 컨테이너와 리소스를 삭제합니다.

Bash

```bash
docker compose down -v
```
