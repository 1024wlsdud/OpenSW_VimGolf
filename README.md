# OpenSW_VimGolf


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
+ 총 타수 : 34
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


|Before|After|
|---|---|
|y1|abs(y1~y4)|
|2,3,4행 lw값|'b','r','g'|
|line #1|line #1~#4|
