# kong-docker-compose
Kong Gateway and Konga 를 위한 Docker Compose 파일입니다.

### 사전공지사항(Disclaimer)
스크립트 내 각종 설정정보(패스워드 및 데이터베이스 명)들이 노출되어 있습니다. 
운영환경에서는 해당 설정 정보들을 별도 분리 보관 하시길 권해드립니다.

### 사전준비사항
아래의 사항들이 설치되어 있어야 합니다.
- Docker
- Docker-compose


### 설치및 실행
```bash
mkdir <스크립트-저장-디렉토리>
cd <스크립트-저장-디렉토리>
git clone https://github.com/Kyungminkim31/kong-docker-compose
sudo docker-compose up
```


### 참고자료
1. [도커 설치가이드] (https://docs.docker.com/get-docker/)
2. [도커콤포즈 설치가이드] (https://docs.docker.com/compose/install/)
2. [콩 게이트웨이 공식 문서] (https://docs.konghq.com/enterprise/?_ga=2.90459608.330569181.1612405671-1374234449.1612405671)
3. [콩가 깃헛 저장소] (https://github.com/pantsel/konga)


### 트러블 슈팅
1. 스크립트 실행은 정상으로 실행되나 콩가 내에서 콩 어드민 로컬 접속이 안될때

    [How to access host port from docker container](https://stackoverflow.com/questions/31324981/how-to-access-host-port-from-docker-container/43541732#43541732)

2. 포트 충돌 문제
    1. 8001, 8443, 1337, 5432 를 사용합니다. 기존의 사용하시는 포트와 충돌시 스크립트 수정을 하여 기동합니다.

