도커 이미지 빌드 & 이미지 레이어
`$ docker build -t 이름/이미지:버전 도커파일의경로`
`$ docker images`

도커 컨테이너 실행
`$ docker run 이름/이미지:버전`

현재 실행중인 컨테이너 확인
`$ docker ps`

실행중인 컨테이너 종료
`$ docekr stop containerID`

실행중인 컨테이너에 특정 액션(컨테이너 ID)
`$ docker exec -it 3884 bash`

도커에서 외부 이미지 불러오기
`$ docker pull busybox`

도커에서 이미지 실행(내부 이미지 검색 -> 외부 이미지 요청)
`$ docker run 이미지이름`

도커 내부 포트 매핑(local PC(호스트)의 80번 포트 : nginx(컨테이너)의 80번 포트)
`$ docker run -p 80:80 nginx`

Volume Mount : 컨테이너 내부의 데이터(폴더)를 호스트의 데이터(폴더)에 마운트 가능
`docker run -v ${PWD}/data:/data/db mongo`

도커를 사용하는 이유 : 지속적 통합(CI, Continuous Integration)
도커를 사용하는 이유 : 지속적 배포(CD, Continuous Deployment)
