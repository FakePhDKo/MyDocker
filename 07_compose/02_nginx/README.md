# Docker Compose: Nginx 포트포워딩 실습📝
## 📖 프로젝트 개요
이 실습은 docker-compose.yml 파일을 사용하여 docker run 명령의 ports 옵션을 변환하고, 컨테이너의 포트를 호스트에 노출하는 방법을 다룹니다.

# 🚀 실습 내용
docker-compose.yml 변환: docker run --name some-nginx -d -p 8080:80 some-content-nginx 명령을 docker-compose.yml 파일의 ports 필드로 변환합니다.

서비스 확인: curl 명령어를 사용하여 호스트의 8080번 포트로 접속하여 Nginx 웹 서버가 정상적으로 서비스되는지 확인합니다.

## 📁 파일 구조

Bash

```bash
.
└── docker-compose.yml
```
