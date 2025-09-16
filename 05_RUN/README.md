# Dockerfile: CMD & ENTRYPOINT 실습📝
## 📖 프로젝트 개요
이 실습은 Dockerfile에서 컨테이너의 메인 프로세스를 정의하는 **CMD**와 ENTRYPOINT 명령의 핵심적인 차이점을 이해하고 활용하는 방법을 다룹니다.

## 🚀 실습 내용
+ CMD의 기본값: CMD ["nginx", "-g", "daemon off;"]와 같이 기본 실행 명령어를 지정하고, docker run 시 명령줄 인자로 이 기본값을 덮어쓸 수 있음을 확인합니다.

+ ENTRYPOINT의 고정 역할: ENTRYPOINT ["top"]과 같이 항상 실행될 명령어를 고정하고, CMD는 ENTRYPOINT의 인자로 사용되는 방법을 학습합니다.

📁 파일 구조
```
.
└── Dockerfile
└── Dockerfile2
```
