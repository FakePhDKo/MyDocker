# Docker 이미지 레이어 구조 파악📝
## 📖 프로젝트 개요
이 실습은 Docker 이미지의 레이어 구조를 깊이 있게 파악하는 과정입니다. Dockerfile의 각 명령어가 어떻게 독립적인 레이어를 형성하는지 직접 빌드하고 분석하여, Docker의 핵심인 레이어 기반 파일 시스템의 원리를 이해합니다.

## 🚀 실습 내용
+ 단계별 빌드: Dockerfile의 명령어를 한 줄씩 추가해가며 여러 버전을 빌드합니다.

+ docker inspect 분석: docker inspect 명령을 사용하여 각 이미지의 RootFS 필드에 기록된 레이어 해시값들을 비교하고, Dockerfile의 각 줄이 새로운 레이어를 생성하는 것을 확인합니다.

## 📁 파일 구조
```
.
├── Dockerfile
├── docker.tar.gz
└── index.html
```
