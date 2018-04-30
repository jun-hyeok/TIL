#Linux Shell Commands
##man
명령어 용법이 기억나지 않을 때

~~~
man <shell command>
~~~

예시

~~~
man ls
~~~

종료 방법 : q

##ls
현재 디렉토리 아래 있는 파일 및 디렉토리 확인

~~~
ls [options] <directory>

-a : 숨겨진 파일 및 디렉토리 전부 나열
-l : 세부 정보 표시 (권한,소유자,크기 등)
-R : 재귀적으로 모든 파일 탐색
-1 : 한 줄에 하나의 항목씩 나열
~~~

##find
디렉토리에서 파일 탐색

~~~
find [options] [path] [expression]

expressions
-name : 해당 이름을 찾음. 패턴 사용 가능
-user : 해당 유저에 속한 파일을 찾음.
-atime : n일 이내 액세스된 파일을 찾음.
-ctime : n일 이내 만들어진 파일을 찾음.
-mtime : n일 이내 수정된 파일을 찾음.
-newer [file] : file보다 최근에 수정된 파일을 찾음.
~~~

##kill
프로세스에 signal을 보냄

~~~
kill -signal [pid]

-9 : kill
-1 : hup. 다시시작
~~~
