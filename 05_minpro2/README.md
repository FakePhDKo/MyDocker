# Docker Mini-Project: Apache + PHP Web Server📝
## 📖 프로젝트 개요
이 프로젝트는 Apache 웹 서버와 PHP 언어가 함께 동작하는 이미지를 제작하는 실습입니다. 단일 컨테이너 내에서 Apache와 PHP-FPM 두 프로세스를 모두 실행하는 방법을 학습하고, Dockerfile의 주요 명령어를 복합적으로 활용합니다.

## 🚀 실습 내용
+ 패키지 설치: httpd, php, php-fpm 등 웹 서버 실행에 필요한 패키지들을 설치합니다.

+ 다중 프로세스 관리: entrypoint.sh 쉘 스크립트를 사용하여 PHP-FPM과 Apache HTTPD를 모두 포어그라운드에서 실행시킵니다.

+ 볼륨과 로그 관리: VOLUME을 사용하여 웹 소스와 로그를 컨테이너 외부에 보존하여 데이터의 영속성을 확보합니다.

## 📁 파일 구조
```
.
├── Dockerfile
├── entrypoint.sh
├── index.html
├── info.php
└── src.tar
```
