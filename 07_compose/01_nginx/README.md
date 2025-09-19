# Docker Compose: Nginx 볼륨 마운트 실습📝
## 📖 프로젝트 개요
이 실습은 docker-compose.yml 파일을 사용하여 docker run 명령의 volumes 옵션을 변환하고, 호스트 디렉터리를 컨테이너에 마운트하여 데이터를 관리하는 방법을 다룹니다.

## 🚀 실습 내용
docker-compose.yml 변환: docker run --name some-nginx -v /some/content:/usr/share/nginx/html:ro -d nginx 명령을 docker-compose.yml 파일의 volumes 필드로 변환합니다.

데이터 관리: 호스트의 ./image-data 디렉터리를 컨테이너에 마운트하여 데이터를 영구적으로 보존하는 방법을 학습합니다.

##📁 파일 구조

Bash

```bash
.
├── docker-compose.yml
└── image-data/
```
