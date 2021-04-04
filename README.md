CyKor-week1 Homework
===========
memory_gosu.cpp memory map(어셈블리에 대한 개념이 아직 약해서 opcode를 사용한 함수 호출과정은 못했습니다.)
------------------------------

STACK 
i, ret, str, str2
------------------
HEAP
-------------------
BSS
ans
----
UNINITIALIZED DATA
num = 1
---------------------
DATA
"\nI am asking you %d time!!!!!\n\n", "No I am not gosu\n", "Yeah.. I am gosu!!\n", "Nah....\n",  "Are you memory gosu?\n",  "Answer : ", "Are you kidding?\n", printf("%s", str),
		printf("%s", str2)
-------------------------------------------------------------------------------------------------------------------------------------------------------------
# calling convention 종류 (차이점은 더 공부를 해야할 것 같습니다.)
push arg는 스택 구조가 arg2 arg1 ret ebp등으로 위에서 아래로 매개변수로 넣어준다.
push Arg2
push Arg1
call func
push ebp
mov ebp
mov esp
leave
ret
# 어셈블리어 
push: 스택에 값을 넣는 것
pop: 스택에 있는 값을 가져오는 것
mov: 단지 값을 넣는 역할
call: 함수를 호출하는 명령어로 뒤에 오퍼랜드로 번지가 붙는다.
CMP: 비교해서 점프하는 명령어
JMP: 비교해서 점프하는 명령어
nop: 아무것도 하지 말라는 명령어
EAX: 더하기, 빼기 등 사칙연산에서 주로 사용됨
INC: i++의 역할을 함
DEC: i--의 역할을 함
AND
OR
int: 인터럽트를 일으키는 명령어
add: src에서 dest로 값을 더하는 명령
sub: src에서 dest로 값을 빼는 명령














