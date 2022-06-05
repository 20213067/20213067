# 오픈소스SW
---
### 리눅스명령어
**1) top : 시스템 사용량을 실시간으로 확인**
- -b : 배치모드로 정보를 출력 
     : 실시간 상화 대화형모드로 정보를 화면에 일렬로 출력
- -n : top 실행 주기를 2번 반복
- -q : 시간의 간격 없이 계속하여 업데이트 정보를 출력

**2) ps : 현재 실행중인 프로세스 목록을 확인, 프로세스의 기본적인 내용만 출력**
- -e : 모든 프로세스를 출력
- -f : 풀 포맷으로 출력(uid, pid, ppid, TTY 등 정보를 보여줌)
- -l : 긴 포맷으로 출력(풀 포맷 + F, S, PRI등 정보를 더 보여줌)
- -p 1 : 프로세스 번호가 1인 프로세스를 출력

**3) jobs : 작업이 중지된 상태, 백그라운드로 진행 중인 작업 상태, 
변경 되었지만 보고되지 않은 상태 등을 표시하는 명령어**
- -l : 프로세스 그룹 ID를 state 필드 앞에 출력
- -n : 프로세스 그룹 중에 대표 프로세스 ID를 출력
- -p : 각 프로세스 ID에 대해 한 행씩 출력
- command : 지정한 명령어를 실행

**4) kill : 프로세스를 죽일 때 사용, 내부적으로는 프로세스에 시그널을 보내 원하는 작업을 하게 하는 명령어**
- -s : 전달할 시그널의 종류를 지정(여기에는 시그널 이름이나 번호를 써준다.)
- -l : 시그널로 사용할 수 있는 시그널 이름들을 보여줌
    (이것은 /usr/include/linux/signal.h 파일에서도 알 수 있다.)
- -1, : -HUP 프로세스를 재활성화
- -9 : 프로세스를 강제로 종료
---
### 매크로 기본 사용법
**매크로 저장하기**
- q<저장할 매크로 문자> -> 매크로 작성 -> q

**매크로 사용하기**
- @<저장한 매크로 문자> -> 반복횟수@<저장한 매크로 문자> -> @@
---
