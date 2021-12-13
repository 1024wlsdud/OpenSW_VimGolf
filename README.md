# OpenSW_VimGolf
# dasasdasd

##VimGolf 문제 솔루션

**1번**
![1번 솔루션](https://user-images.githubusercontent.com/43934522/144701855-96d20908-45c5-47a7-a91b-0f2819b84b03.gif)

{{ }} 를 "{{ }}"로 만드는 문제


+ 총 타수 : 9
+ WriteUP
1. } - 문단의 끝으로 이동 
2. % - 괄호의 짝 찾아 이동
3. i - 입력모드
4. " 입력
5. END - 라인 끝으로 이동
6. " 입력
7. ESC 입력으로 명령모드
8. ZZ로 저장 후 나가기 


**2번**
![2번 솔루션](https://user-images.githubusercontent.com/43934522/144702760-ede2617d-06f5-462d-a0b3-47d2ad3a7c2f.gif)


sublime과 emacs를 vim으로 치환하는 문제
+ 총 타수 : 27
+ WriteUP
1. :%s/sublime|emacs/vim/g => sublime 또는 emacs를 vim으로 교체, g는 라인 여러개 치환 
2. ZZ로 저장 후 나가기 

**3번**
![3번](https://user-images.githubusercontent.com/43934522/144706269-97ce5597-ae65-4e50-9a17-985dc2441c16.gif)


var 안에 주석 Version TODO와 Debug TODO 삽입
+ 총 타수 : 34 (어떻게 20을..?)
+ WriteUP
1. 4G - 4번째 행으로 이동
2. yw - 커서가 있는 단어를 복사(Version)
3. O - 커서가 있는 라인을 한 줄 내리고 입력모드로 변환
4. // 입력 후 스페이스바로 공백 만듦
5. ESC - 명령모드 변환
6. p - yw로 복사한 단어 붙여넣기
7. a TODO - 커서 뒤에 입력모드 변환 후 TODO입력
8. ESC - 명령모드 변환
9. 6G - 6번째 행 이동
10. yw - 커서가 있는 단어 복사(Debug)
11. O - 커서가 있는 라인을 한 줄 내리고 입력모드로 변환
12. // 입력 후 스페이스바로 공백 만듦
13. ESC - 명령모드 변환
14. p - yw로 복사한 단어 붙여넣기
15. a TODO - 커서 뒤에 입력모드 변환 후 TODO입력


**4번**
![image](https://user-images.githubusercontent.com/43934522/144706317-93bce532-b92a-4e6b-b337-f82bf638b214.png)
![4번 솔루션](https://user-images.githubusercontent.com/43934522/144720144-41df3791-d23b-4811-a9df-ae455d3eba0d.gif)


|Before|After|
|---|---|
|y1|abs(y1~y4)|
|3,4,5행 lw값|'b','r','g'|
|line #1|line #1~#4|

+ 총 타수 : 57
+ WriteUP
1. /y - y를 abs(y~)형태로 바꾸기 위해선 y위치를 찾아야 함. /y를 통해 y의 위치를 찾음
2. Enter - Enter로 해당 y위치에 커서 이동
3. cw - y를 지우고 abs(y1) 작성
4. ESC - 명령모드로 변경
5. N - N으로 맨처음 명령모드에서 y를 검색했던걸 재검색
6. . - .으로 3번(cw~)실행
7. 5~6번을 반복 실행한 후 만들어진 4개의 abs(y1)를 편집모드로 들어가 2, 3, 4 로 변경
8. ESC - 명령모드로 변경
9. /k - k의 위치 찾은 후 ENTER로 커서 이동
10. s - 해당 단어를 지우고, 입력모드로 변경
11. 방향키와 벡스페이스바 키를 이용해 k를 b, r, g를 작성
12. ESC - 명령모드로 변경
13. /# - #뒤에 있는 숫자를 변경하기 위해 #를 검색
14. a - #앞으로 커서 이동 후 입력모드로 변경 후, 2, 3, 4를 작성


**5번**
![5번 솔루션](https://user-images.githubusercontent.com/43934522/144721416-e87a48d4-078a-4665-8ff9-3e6e3453bd0c.gif)
+ 총 타수 : 27
+ WriteUP
1. 5G - 5번 째 행 이동
2. yw - student_id 복사
3. /" - "검색
4. p - 복사한 내용 붙여넣기
5. a - 커서 앞으로 입력모드 변경 후, name, age, score작성 
6. ESC 누른 후, ZZ로 빠져나가기 
