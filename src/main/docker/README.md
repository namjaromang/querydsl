# brew가 없나요?
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 도커설치 (mac 기준입니다.)

brew install docker brew install docker-compose

# 권한부여

sudo chmod +x /usr/local/bin/docker-compose

# 실행 ( -d 백그라운드 모드 옵션 입니다.)
docker-compose -f src/main/docker/mysql-test.yml up -d 

#도커 프로세스 확인
docker ps

#로그 확인
docker logs {container ID}

#컨테이너 정지
docker stop {cont