## 리스트(배열) & 딕셔너리(객체)
리스트를 배열(Array)이라고도 부릅니다
리스트: 순서를 지켜서 가지고 있는 형태입니다.

``` js
let b_list = [1,2,'hey',3] // 로 선언 가능
b_list[1] // 2 를 출력
b_list[2] // 'hey'를 출력
```

값을 추가하고 싶을때

``` js
b_list.push('헤이')
b_list // [1, 2, "hey", 3, "헤이"] 를 출력
```

리스트의 길이 구하기
```
b_list.length // 5를 출력
```

- 딕셔너리: 키(key)-밸류(value) 값의 묶음
    
    <aside>
    👉 딕셔너리는 객체로도 불립니다
    
    </aside>

``` js
let b_dict = {'name':'Bob','age':21} // 로 선언 가능
b_dict['name'] // 'Bob'을 출력
b_dict['age'] // 21을 출력

b_dict['height'] = 180 // 딕셔너리에 키:밸류 넣기
b_dict // {name: "Bob", age: 21, height: 180}을 출력
```

## 딕셔너리의 자주쓰는 또 다른 표현
let b_dict = {'name':'Bob','age':21}

//bob 이름을 꺼낼땐 두 가지 방식으로 깞을 꺼낼 수 있습니다.
b_dict['name']
b_dict.name //연결연산자

둘다 똑같이 딕셔너리의 키값에 접근하여 값을 꺼내옵니다.

## 리스트와 딕셔너리가 왜 필요할까요?
    💡 **순서를 표시할 수 있고, 정보를 묶을 수 있습니다.**

    변수만을 사용한 모습
       
``` js
        let customer_1_name = '박씨';
        let customer_1_phone = '010-1234-1234';
        let customer_2_name = '김씨';
        let customer_2_phone = '010-4321-4321';
            ...(알아보기 힘듬)
```

    👉딕셔너리를 활용한다면 다음과 같이 고객 별로 정보를 묶을 수 있습니다.
   
``` js

        let customer_1 = {'name': '박씨', 'phone': '010-1234-1234'};
        let customer_2 = {'name': '김씨', 'phone': '010-4321-4321'};
```

    👉그리고 순서를 나타내기 위해 리스트를 사용하면, 이렇게나 깔끔해집니다.
    let customer = [
        {'name': '김스파', 'phone': '010-1234-1234'},
        {'name': '박르탄', 'phone': '010-4321-4321'}
    ]
    
    ✅보기에도 깔끔해지고, 다루기도 쉬워지고, 고객이 새로 한 명 더 오더라도 .push 함수를 이용해 간단하게 대응할 수 있습니다.
    

나눗셈의 나머지를 구하고 싶은 경우

```
let a = 20
let b = 7

a % b = 6
```

모든 알파벳을 대문자로 바꾸고 싶은 경우

```
let myname = 'spartacodingclub'

myname.toUpperCase() // SPARTACODINGCLUB

👉 console.log(myname.toUpperCase())
```

또, 특정 문자로 문자열을 나누고 싶은 경우 1

let myemail = 'sparta@gmail.com'

let result = myemail.split('@') // ['sparta','gmail.com']

result[0] // sparta
result[1] // gmail.com

let result2 = result[1].split('.') // ['gmail','com']

result2[0] // gmail -> 우리가 알고 싶었던 것!
result2[1] // com

함수형 프로그래밍 : 연결해서 쓰기
myemail.split('@')[1].split('.')[0] // gmail -> 간단하게 쓸 수도 있다!

특정 문자로 나누고 싶은 경우 2

let txt = '서울시-마포구-망원동'

let names = txt.split('-'); // ['서울시','마포구','망원동'

특정 문자로 합치고 싶은 경우

let result = names.join('>'); // '서울시>마포구>망원동' (즉, 문자열 바꾸기!)