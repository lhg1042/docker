

docker desktop 설치, docker hub 회원가입 후

-mysql image 생성
docker pull mysql:8.0.22 

-docker 로그인
docker login -u hyegyulee
Password: (입력)
=> Login Succeeded

-docker images #image 확인

-docker hub push
docker tag mysql:8.0.22 hyegyulee/hyegyu-repository:v1.0.0
docker push hyegyu-repository:v1.0.0

![repository image](https://user-images.githubusercontent.com/65995264/204120147-7d8b5f5b-8a9b-4d2c-b180-7f129c4592ce.png)

-dockercompose
docker-compose.yml 파일 작성 후 커맨드
docker-compose up -d

-mysql 접속
docker exec -it mysql-test bash
mysql -u root -p 
Enter password: (패스워드 입력)

table 생성 후 1) 상품 정보 : 상품명, 금액, 등록일자, 등록업체명 조회
![test](https://user-images.githubusercontent.com/65995264/204120437-653f18f5-223f-4330-9852-8fcf0df57753.png)





