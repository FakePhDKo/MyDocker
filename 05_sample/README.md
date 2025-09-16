# Dockerfile: 기본 사용법 및 빌드 캐싱📝
## 📖 프로젝트 개요
이 프로젝트는 가장 기본적인 Dockerfile을 작성하고, 이미지를 빌드 및 재빌드하는 과정을 통해 Docker 빌드 시스템의 캐싱 원리를 이해합니다. 이를 통해 빌드 시간을 단축하는 방법을 학습합니다.

## 🚀 실습 내용
+ 기본 이미지 빌드: FROM 명령만 포함된 Dockerfile을 빌드하여 기본 이미지를 생성합니다.

+ 이미지 캐싱: 동일한 Dockerfile을 다시 빌드할 때, Docker가 이미 다운로드한 레이어를 재사용하여 빌드 과정이 매우 빨라지는 것을 확인합니다.

+ 표준 입력 빌드: tar로 묶어 표준 입력으로 빌드하는 방식도 실험하지만, 실무에서는 권장되지 않음을 학습합니다.

📁 파일 구조
```
.
├── Dockerfile
├── Dockerfile1
├── Dockerfile2
├── Dockerfile3
├── Dockerfile4
├── dummyfile
├── hello docker
├── index.html
└── docker.tar.gz
```
