# Dockerfile: RUN 명령 형식 비교📝
## 📖 프로젝트 개요
이 실습은 Dockerfile의 RUN 명령에서 사용되는 두 가지 형식인 Shell 형식과 Exec 형식의 차이점을 명확히 비교합니다. 이를 통해 명령어의 실행 방식과 보안상의 이점을 이해합니다.

## 🚀 실습 내용
+ Shell 형식: RUN echo '...'와 같이 일반적인 터미널 명령어 형태로 실행합니다.

+ Exec 형식: RUN ["echo", "..."]와 같이 배열 형태로 명령과 인자를 분리하여 실행합니다.

+ 상세 로그 분석: docker build --progress=plain 명령어를 통해 각 형식의 빌드 과정과 레이어 생성 방식을 관찰합니다.

##📁 파일 구조
```
.
└── Dockerfile2.txt
```
