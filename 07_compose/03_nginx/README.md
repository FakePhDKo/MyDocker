# Docker Compose: Nginx 설정 파일 마운트 실습📝
## 📖 프로젝트 개요
이 실습은 docker-compose.yml 파일을 사용하여 nginx 컨테이너에 호스트의 설정 파일을 마운트하는 방법을 다룹니다. command 옵션을 사용해 nginx 서버의 실행 방식을 변경하는 방법도 함께 학습합니다.

## 🚀 실습 내용
+ docker-compose.yml 변환: docker run -p 80:80 -v $(pwd)/nginx.conf:/etc/nginx/nginx.conf:ro nginx 명령을 docker-compose.yml 파일의 volumes와 command 필드로 변환합니다.

+ 설정 파일 마운트: 호스트에 있는 nginx.conf 파일을 컨테이너에 마운트하여, 컨테이너의 설정을 호스트에서 관리하는 방법을 익힙니다.

+ command 옵션: nginx-debug -g 'daemon off;'와 같은 명령어를 command 필드로 변환하여 컨테이너의 메인 프로세스를 제어하는 방법을 학습합니다.

## 📁 파일 구조

Bash

```bash
.
├── docker-compose.yml
└── nginx.conf
```
