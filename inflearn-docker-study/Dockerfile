# OS 셍상(centos:7)
# FROM 명령어 -> 이미지
FROM centos:7

# 작업 dir 전환
# WORKDIR /app

# COPY A B : A 파일을 B에 복사
# . 은 컨테이너 내부 dir(root dir)
COPY name.txt .

# CMD : 쉘 명령어 실행
# CMD cat name.txt
CMD while true; do sleep 3; cat name.txt; done;

