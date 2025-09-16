# Dockerfile: WORKDIR 명령 실습📝
## 📖 프로젝트 개요
이 실습은 Dockerfile에서 WORKDIR 명령을 사용하여 작업 디렉터리를 설정하는 방법을 학습합니다. 연속된 WORKDIR 사용과 ENV 환경 변수를 결합하여 사용하는 두 가지 방법을 비교하고, 권장되는 방식을 알아봅니다.

## 🚀 실습 내용
+ WORKDIR 연속 사용: WORKDIR /app/sub와 같이 여러 번 디렉터리를 지정하여 작업 경로를 변경합니다.

+ ENV + WORKDIR: ENV APP_DIR /app와 같이 환경 변수를 사용해 WORKDIR를 지정하여 가독성과 유지보수성을 높이는 방법을 실습합니다.

📁 파일 구조
```
.
└── Dockerfile
```
