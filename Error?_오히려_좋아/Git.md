7월 13일 수요일
``` terminal
Agreeing to the Xcode/iOS license requires admin privileges, 
please re-run as root via sudo
```

라는 오류가 뜨면
 
> ## *해결 방법*

1. 터미널을 연다.

2. `sudo xcodebuild -license` 을 입력한다.
```
You have not agreed to the Xcode license agreements. 
You must agree to both license agreements below in order to use Xcode. 
Hit the Enter key to view the license agreements at 
'/Applications/Xcode.app/Contents/Resources/English.lproj/License.rtf'
```
3. return 키를 누르면 약관 페이지가 출력된다.
4. q를 눌러 종료 시키면
5. 
```
By typing 'agree' you are agreeing to the terms of the software 
license agreements. Type 'print' to print them or anything else 
to cancel, [agree, print, cancel]
```
위 메시지가 뜬다.
그러면  "agree"라고 입력하면 해결 끝!

</br>

### 출처 [개발개발개발:티스토리](https://devinside.tistory.com/138)
