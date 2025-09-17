# Python Application with MySQL on Docker📝
## 📖 프로젝트 개요
이 프로젝트는 두 개의 독립된 컨테이너를 사용하여 마이크로서비스 아키텍처의 기본 원리를 경험하는 실습입니다. Flask 웹 애플리케이션 컨테이너와 MySQL 데이터베이스 컨테이너를 구축하고, 네트워크와 볼륨을 활용하여 이들을 연동합니다.

## 🚀 실습 내용
+ Flask 애플리케이션 컨테이너화: 파이썬 가상 환경에서 테스트한 Flask 애플리케이션을 Dockerfile로 빌드합니다.

+ 다중 컨테이너 구성: 웹 서버와 DB를 분리된 컨테이너로 실행하고, **docker volume**을 통해 데이터 영속성을 확보합니다.

+ 컨테이너 통신: **docker network create**로 사용자 정의 네트워크를 만들어 컨테이너 이름(예: mysqldb)으로 통신하는 방법을 실습합니다.

```
📁 파일 구조
.
├── __pycache__
├── custom_flask_env (가상환경)
├── app.py
├── requirements.txt
└── Dockerfile
```
