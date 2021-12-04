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
