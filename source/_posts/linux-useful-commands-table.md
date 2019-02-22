---
title: 리눅스 유용한 명령어 모음
---

| purpose | exmaple | comment |
| ------- | ------- | ------- |
| rsync   | `$ rsync --info=progress2 source dest` | 진행상황을 출력하면서 파일 전송 |
| curl    | `$ curl -o naver https://www.naver.com/` | 진행상황을 출력하면서 다운로드 진행 |
| 배포판 버전체크 | `$ cat /etc/issue` | |
| 배포판 이름확인 | `$ cat /etc/*-release`| |
| 프로세스 보기 | `$ ps -ef` `$ ps -ef | grep ${keyword}` | |
| 로그 실시간 출력 | `$ tail -F /var/log/nginx/access.log` | |
| 포트 체크하기 | `$ netstat -nlp` | 또는 `$ nmap` 패키지로 확인 가능 |
| CPU 코어 갯수 확인 | `$ cat /proc/cpuinfo | grep processor | wc -l` | |
| *hostname* 변경 | `$ vim /etc/hostname` | |
| (*\**) php7 관련 파일 지우기 | `$ find / -name php7* -exec rm -rf {} \` | 응용 사용 |
| *service* 리스트 | `$ ls /etc/rc*.d` or `$ service --status-all` | |
| (*\**) benchmark | `$ ab -c 10 -n 1000 -k http://localhost/xe-core/` | 동시 접속자 수 10명으로 1,000번의 요청을 시도한다. |