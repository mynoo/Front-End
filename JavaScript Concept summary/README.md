<div align="center" id="top">
<img height="270px" width="270px" src="./logo.png"><br>
  <h1>📃개념 및 궁금증 정리</h1>
</div>

***
## 자동 실행 함수
**window.onload**
- 페이지가 로드되면 자동으로 실행되는 함수를 구현할 때 사용
- 모든 요소들이 로드된 이후에 호출된다.
- 한 페이지에서 하나의 window.onload()함수만 적용된다.
```
window.onload = function(){
  자바스크립트 코드....
}
```

**(document).ready()**
- window.onload함수의 문제점을 해결하기 위해 사용하는 함수
- 외부 리소스 및 이미리 로딩과 상관없이 DOM 요소들만 로드되면 호출된다.
- 중복 사용해도 순서대로 모두 실행된다.
```
${document}.ready(function(){

});
```

## 제이쿼리(jQuery)란?
오픈소스기반의 자바스크립트 라이브러리
- 제이쿼리를 사용하면 짧고 단순한 코드로도 웹 페이지에 다양한 효과나 연출을 적용할 수 있다.

## 배열 요소 추가, 삭제

**배열 요소 추가**
```
var arr = ['a', 'b', 'c'];

// arr = ['a', 'b', 'c', 'd']
arr.push('d'); // 배열의 끝에 요소를 추가
```

```
var arr = ['a', 'b', 'c'];

// arr = ['d', 'a', 'b', 'c']
arr.unshift('d'); // 배열의 앞쪽에 요소를 추가
```

```
var arr = ['a', 'b', 'c'];

// arr = ['a', 'b', 'd', 'c']
arr.splice(2, 0, 'd'); // index 2 ('c')의 위치에 요소를 추가
```

**배열 요소 삭제**
```
var arr = ['a', 'b', 'c', 'e', 'f'];

// arr = ['a', 'b', 'c', 'e']
arr.pop(); // 배열의 마지막 요소를 제거
```

```
var arr = ['a', 'b', 'c', 'e', 'f'];

// arr = ['b', 'c', 'e', 'f']
arr.shift(); // 배열의 첫번째 요소를 제거
```

```
// arr = ['a', 'b', 'e', 'f']
arr.splice(2, 1); // index 2 부터 1개의 요소('c')를 제거
```
