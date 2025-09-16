# Dockerfile: ONBUILD 명령 실습📝
## 📖 프로젝트 개요
이 실습은 ONBUILD 명령을 사용하여 이미지 빌드 과정을 자동화하는 방법을 배웁니다. ONBUILD가 포함된 템플릿 이미지를 만들고, 이 이미지를 기반으로 실제 애플리케이션 이미지를 빌드하는 과정을 통해 자동화의 원리를 이해합니다.

## 🚀 실습 내용
+ ONBUILD가 포함된 Dockerfile.base를 빌드하여 템플릿 이미지를 생성합니다.

+ FROM web-base 한 줄만으로 ONBUILD에 정의된 모든 작업(웹 콘텐츠 복사 등)이 자동으로 실행됨을 확인합니다.

+ docker inspect 명령으로 ONBUILD 명령이 이미지 메타데이터에 어떻게 기록되는지 분석합니다.

## 📁 파일 구조
dockertext2는 https://github.com/asashiho/dockertext2에서 clone한 폴더입니다.
```
.
├── dockertext2
├── website
├── Dockerfile
├── Dockerfile.base
└── website.tar
```
