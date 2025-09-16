# Docker Essentials 📝
## 📖 프로젝트 개요
이 저장소는 도커 컨테이너 기술의 핵심 개념과 실무 응용을 학습한 결과물입니다. Dockerfile을 이용한 이미지 빌드부터, 네트워킹, 데이터 관리, 그리고 다양한 패키지 관리 도구 활용까지, 도커의 기본기를 체계적으로 다루고 있습니다.

각 디렉터리는 독립적인 실습 모듈로 구성되어 있으며, 단순히 명령어를 나열하는 것을 넘어 기술적인 원리를 이해하고 문제를 해결하는 과정을 담고 있습니다.

## 📂 프로젝트 구조
이 저장소는 다음과 같은 디렉터리로 구성되어 있습니다. 각 디렉터리에는 실습 스크립트와 상세한 설명을 담은 README.md 파일이 포함되어 있습니다.

+ 05_dockerfile/: RUN 명령의 Shell vs. Exec 형식 비교 실습.

+ 05_ImageLayer/: Docker 이미지 레이어 구조 파악 실습.

+ 05_MultiStage/: 멀티 스테이지 빌드 전략 실습.

+ port-forwarding-practice/: 포트 포워딩의 원리 및 필요성 실습.

+ 05_RUN/: CMD와 ENTRYPOINT 명령 사용법 실습.

+ 05_onbuild/: ONBUILD를 사용한 이미지 빌드 자동화 실습.

+ 05_workdir/: WORKDIR 명령 사용법 실습.

## 🚀 주요 실습 내용
+ Docker 설치 자동화: install_docker.sh와 restore_install_docker.sh를 통해 환경 구축을 자동화했습니다.

+ 이미지 레이어: docker build --progress=plain과 docker history를 통해 이미지의 레이어 구조와 빌드 과정을 깊이 있게 분석했습니다.

+ 네트워킹: 포트 포워딩(-p), 사용자 정의 네트워크(docker network create)를 통해 컨테이너의 통신 원리를 이해하고 **ping: bad address**와 같은 문제를 해결했습니다.

+ 데이터 관리: 볼륨(docker volume)과 바인드 마운트(-v)를 비교하며 컨테이너 데이터의 영속성을 확보하는 방법을 익혔습니다.

+ Dockerfile 심화: RUN 명령의 두 가지 방식(Shell vs. Exec), CMD와 ENTRYPOINT의 차이, ONBUILD와 WORKDIR의 실무적 활용법을 학습했습니다.

## 🛠️ 실행 방법
각 디렉터리로 이동하여 README.md 파일의 안내에 따라 실습 스크립트를 실행해 보세요.
