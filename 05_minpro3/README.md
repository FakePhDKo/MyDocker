# Docker Mini-Project: Apache + Python WSGI Server📝
## 📖 프로젝트 개요
이 프로젝트는 Apache 웹 서버와 **Python WSGI(Web Server Gateway Interface)**를 결합한 이미지를 제작하는 실습입니다. mod_wsgi를 활용하여 웹 서버와 파이썬 애플리케이션 간의 효율적인 통신을 구축하고, 컨테이너화하는 과정을 다룹니다.

## 🚀 실습 내용
+ WSGI 컨테이너화: mod_wsgi를 설치하고 vhost.conf, myapp.wsgi와 같은 설정 파일을 컨테이너에 복사하여 WSGI 환경을 구축합니다.

+ 데이터 분리: 웹 콘텐츠와 로그를 별도의 볼륨에 마운트하여 데이터의 영속성을 확보합니다.

+ 서비스 테스트: 웹 브라우저를 통해 WSGI 애플리케이션에 정상적으로 접근하여 "Hello World!"가 출력되는 것을 확인합니다.

## 📁 파일 구조
```
.
├── Dockerfile
├── myapp.wsgi
└── vhost.conf
```
