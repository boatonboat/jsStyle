# 자바스크립트 프로그래밍 스타일

```
language : (kr)
작성자 : 보트
읽는데 걸리는 시간 : 약 7분
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

