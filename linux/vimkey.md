# **vi의 모드**
## 일반모드  
vi의 명령키를 기다리는 상태 
## 입력모드  
텍스트를 입력하는 모드. 일반모드에서 a,i,o,O등의 키입력으로 전환. 
## 명령모드  
ESC로 일반모드로 돌아감.

## 입력모드로 전환  

|종류|기능|
|---|:---:|
|'a'|append. 현재 커서 위치에서 한 칸 뒤로 이동하고 입력모드 전환|
|'A'|현재 행 끝으로 이동 후 입력모드 전환|
|'i'|insert. 현재 커서 위치에서 입력모드 전환|
|'I'|현재 행 맨 앞으로 이동 후 입력모드 전환|
|'o'|open line. 현재 행 아래 새로운 행을 하나 만들고 입력모드 전환|
|'O'|현재 행 위에 새로운 행을 하나 만들고 입력모드 전환|
|'R'|Replace. 수정모드. 기존 글자 위에 덧쓰여진다|  

## 저장과 종료(명령 모드에서)  

|종류|기능|
|---|:---:|
|':w'|저장|
|':wq','x'|저장 후 종료|
|':q!'|강제 종료(저장하지 않고)|
|'w filename'|filename으로 파일 저장(사본 저장 기능)|
|'w../filename'|부모 디렉토리에 파일 저장|
|'w! filename'|강제로 덮어쓰기|  

## 커서 이동  

|종류|기능|
|---|:---:|
|'h,j,k,l'|순서대로 왼,아래,위,오른|
|'[#]h,j,k,l'|왼쪽에 숫자가 있으면 그 숫자 칸 만큼 이동|
|'^'|행 맨 앞으로 이동|
|'$'|행 맨 뒤로 이동|
|'Crtl + B / Crtl + F'|Back/Forward 한 화면 위/아래 이동|
|'Crtl + U / Crtl + D'|Up/Down 화면의 절반씩 위/아래 이동|
|'[#]G'|숫자에 해당하는 행으로 이동, 숫자가 생략되면 맨 아래 행으로 이동|
|'gg'|첫번째 행으로 이동|
|'w'|words forward. 단어의 시작위치를 단위로 이동|
|'e'|end of word. w와 비슷하지만 단어의 끝 위치 단위로 이동|
|'b'|words backward. w처럼 움직이지만 역방향으로|  

## 현재 위치 확인하기  

|종류|기능|
|---|:---:|
|'file'|-명령행 모드에서 현재 파일 어느 위치에 커서가 있는지 확인|
|'Crtl+G'|-일반 모드에서 현재 파일 어느 위치에 커서가 있는지 확인|  

## 복사/붙여넣기  

|종류|기능|
|---|:---:|
|'yy'|현재 행 복사하기|
|'dd'|현재 행 잘라내기|
|'p'|현재 행 위쪽에 붙여넣기|
|':%y'|문서 전체 복사|
|'5,10y'|5번째 행부터 10번째 행까지 복사|
|':.,+10y'|현재 행부터 아래로 10행 복사|  

## 삭제하기  

|종류|기능|
|---|:---:|
|'x'|문자 삭제|
|'dd'|현재 행 삭제|  

## 비주얼모드  

**시각적으로 보면서 블록을 잡는 기능**
'v' 현재 위치부터 블록 설정
