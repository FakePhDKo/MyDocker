# Docker Mini-Project: FTP Server📝
## 📖 프로젝트 개요
이 프로젝트는 FTP(Active Mode) 서버로 동작하는 커스텀 이미지를 직접 제작하는 실무 실습입니다. Dockerfile의 다양한 명령어를 조합하여 안정적인 FTP 서버를 컨테이너화하고, 외부 접속 테스트까지 진행합니다.

## 🚀 실습 내용
+ FTP 서버 설치: vsftpd 패키지를 설치하고, 익명 FTP를 위한 설정을 컨테이너에 적용합니다.

+ Active Mode 설정: FTP의 데이터 포트(20/tcp)와 제어 포트(21/tcp)를 명시적으로 노출하여 Active Mode 연결을 지원합니다.

+ 볼륨 및 네트워크: /var/ftp/pub 디렉토리에 볼륨을 마운트하고, 사용자 정의 네트워크에 컨테이너를 연결합니다.

+ 실행 프로세스 정의: ENTRYPOINT 명령을 사용하여 컨테이너의 메인 프로세스를 vsftpd로 고정합니다.

## 📁 파일 구조
```
.
├── Dockerfile
├── WelcomeToMyFTPServer.txt
└── vsftpd.conf.template
```
