### python-assignment_3
# 리녹스 명령어 *top,ps,jobs,kill* 명령어 조사
___

## 1. top
(1) 주요 기능
* 시스템의 CPU, 메모리, 스왑, 프로세스 정보 등을 실시간으로 업데이트하여 표시
* 실행 중인 프로세스를 확인하고, 우선순위를 변경하거나 종료
* CPU, 메모리, 스왑 등 시스템 자원의 사용률을 확인
* CPU 사용률, 메모리 사용률, 실행 시간 등을 기준으로 프로세스를 정렬

(2) 실행 옵션
* **-b**: 순간 정보 확인(batch 모드)
* **-n**: top 실행 주기 설정(반복 횟수)

(3) 실행 후 명령어
* **shift + p**: CPU 사용률 내림차순
* **shift + m**: 메모리 사용률 내림차순
* **shift + t**: 프로세스가 돌아가고 있는 시간
* **a**: 메모리 사용량에 따라 정렬

(4) 실행 예시
> **top -b -n 1**
![image](https://uc0cb0c24501f3ad48a032e1ef19.dl.dropboxusercontent.com/cd/0/inline/CsM8izNrcJmkIkamrr04BDEo2X2iIqk-jsRRw5Wp_q2xXTFLG88zd9chqj3QwiBgo5-ni8t6URuP2VFgc1mle9p96sJfMVermU8v1wK_V-KKyBBuqYD9IcNftxK7LqAZkd0bsbD9ThjjcBsL9pY1p7Yu/file#)

___

## 2. ps
(1) 주요 기능
: 현재 구동 중인 프로세스 정보 확인

(2) 실행 옵션
- **-e**: 현재 사용자 뿐만 아니라 다른 사용자들이 구동시킨 모든 프로세서를 보여줌.
- **-f**: 보다 상세한 정보를 보여줌 *(Full format)* 
- **-l**: -f 보다 **더** 상세한 정보를 보여줌 *(Long format)*

(3) 실행 예시
> **ps -ef | head**
![image](https://postfiles.pstatic.net/MjAyMTA0MjVfMjQ0/MDAxNjE5MzQ0Nzk0NDU3.sV5NU5mf6Tg4j97sNOl7Y9KSfT6gZI-9ZRvSd3YnOlUg.8QpSoyjeBKfC9BfqkOOapEEXKkx4IuWseMuRzX3JY9Yg.PNG.tmk0429/ps_ef.png?type=w773)

___

## 3. jobs
(1) 주요 기능
+ 현재 쉘 세션에서 실행 중이거나 일시 중지된 작업을 확인할 때 사용
+ 각 작업에 대해 작업 번호, 프로세스 ID, 작업 상태, 명령어 이름 등을 출력

(2) 실행 옵션
|명령어|역할|
|:--:|:--:|
|-l|각 작업의 프로세스 ID(PID)도 함께 출력|
|-p|작업의 프로세스 ID만 출력|
|-n|가장 최근에 상태가 변경된 작업만 출력|
|-r|실행 중(Running)인 작업만 출력|
|-s|일시 중지된 작업만 출력|

(3) 실행 예시
Click [here](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdna%2F6y8AH%2Fbtsy9N0jKrh%2FAAAAAAAAAAAAAAAAAAAAAEm7P4LNovSheVghu3KP7WrwzLslJirHcITBGVnaujpp%2Fimg.png%3Fcredential%3DyqXZFxpELC7KVnFOS48ylbz2pIh7yKj8%26expires%3D1751295599%26allow_ip%3D%26allow_referer%3D%26signature%3DEURUlROgEHP4DWq0MB7sfHRzSRE%253D)

___

## 4. kill
>  ***특정 프로세스나 프로세스 그룹에 시그널을 보내 프로세스를 종료하는 데 사용***
>
> **kill [옵션] <프로세스 ID>**
* [옵션]: 명령어의 동작을 제어하는 옵션을 지정
* <프로세스 ID>: 종료하고자 하는 프로세스의 고유 식별자인 프로세스 ID를 지정

### 실행 예시 ###
![image](https://mblogthumb-phinf.pstatic.net/MjAyMTA0MjVfMTcg/MDAxNjE5MzQ4MzIxNTQz.fnoYAdBVIOnrRhgeiuEpv-tysNuPgslXAFsyw4uXHP4g.Nd3d22pKdbH9XUnbLxTSk5dwRP-7OCYH5JoQkVglprMg.PNG.tmk0429/%EB%8B%A8%EC%88%9C_kill.png?type=w800)


