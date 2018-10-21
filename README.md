# 자바스크립트 프로그래밍 스타일

```
language : (kr)
작성자 : 보트
읽는데 걸리는 시간 : 약 7분
언어 번역자를 찾고 있습니다.
```

#### 변수 선언 (1)
``` js
// GOOD
var a = 10;
var b = 10
var c = 10;
// BAD
var a=10,b=10,c=10;
```

#### 매개변수 접속사 사용
```js
//ex 첫글자 대문자 , 접속사 사용
// GOOD
function a(x_,y_){
   var x = x_;
   var y = y_;
}
// BAD
function a(functionx,functiony){
  var x = functionx;
  var y = functiony;
}
```
#### 들여쓰기 사용
```js
// + 들여쓰기는 스페이스 또는 탭 사용
// GOOD
for(var i=0;i<10;i++){
    if(i==2){
       console.log(i);
    }
}
// BAD
for(var i=0;i<10;i++){
if(i==2){
console.log(i);
}
}
```
#### 변수에 관련 있는 이름 사용
```js
// GOOD
var appleCount = 0; 
var mouserotaion = 0;
// BAD
var a = 0;
var r = 0;
```
#### 세미콜론 사용
```js
// GOOD
var a = 10 + 2 + 3;
console.log("Hello World"+a);
// BAD
var a = 10 + 2 + 3
console.log("Hello World"+a)

//ex 코드를 압축했을때 인터프리터가 코드를 구분 할 수 없다.
```
#### 비슷한 변수 이름 사용 X
```js
// GOOD
var x = 1000;
var xcount = 0;
// BAD
var x = 1000;
var x2 = 0;
```
#### if문 한줄일때 중괄호 생략
```js
// + 실행할 코드가 한 줄일때는 중괄호 생략 O
// GOOD
if(a==b)
   console.log(a,b);
// BAD
if(a==b){
   console.log(a,b);
}
```
# 꿑팁
#### 크롬 console을 자주 이용
```js
// + 크롬 콘솔은 생각보다 기능이 많다
// + F12 또는 ctrl+ shift + i 로 콘솔창 킬 수 있음
console.log("1.2.3"); // 콘솔 출력

console.table([1,2,3,4,5]); // 콘솔 Array 출력

console.time('timer');// 타이머 시작
for(var i=0; i < 1000; i++){
  1+1;
}
console.timeEnd('timer'); //타이머 종료
```
=실행화면
![image](https://user-images.githubusercontent.com/43812153/47266003-3445b280-d56b-11e8-9bff-488fedfc0b1c.png)
