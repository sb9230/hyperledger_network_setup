# hyperledger_network_setup

docker 설치

sudo atp-get update
sudo rm -rf /경로/
sudo atp-get install docker.io
sudo atp-get software-properties-common

현재 접속중인 사용자에게 권한 주기

sudo usermod -aG docker $USER

#rebooting

sudo reboot

#rebooting 후 버전확인
docker version

curl 설치
sudo apt-get install curl

node.js 설치

sudo apt-get update
sudo apt-get install build-essential libssl-dev

go 설치

curl -O https://storage.googleapis.com.golang/go1.12.17.linux-amd64.tar.gz
//설치할 버전 넣기

tar-xvf go1.12.17.linux-amd64.tar.gz

1. 준비물 생성
crypto-config.yaml
configtx.yaml
genetate.sh

2. 네트워크 수행
docker-compose.yaml
start.sh

3.채널 join
start.sh
peer channel create
peer channel join

디렉토리 구조 만들기
mkdir sample-network
cd sample-network
mkdir application network contract
cd ~/fabric-samples/basic-network
cp .env crypto-config.yaml configtx.yaml generate.sh docker-compose.yml start.sh teardown.sh ~/dev/sample-network/network

