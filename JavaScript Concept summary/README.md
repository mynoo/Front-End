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

<div align="center" id="top">
  <h1>함수 모음</h1>
</div>
:::Window객체:::

- window.defaultStatus▶ 상태 표시줄에 표시할 문자열의 초기 값 설정
- window.frames▶ 창에 포함된 프레임을 배열 형태로 지정
- window.opener▶ 오픈메소드를 사용해서 새 상츨 열었을 경우, 새 창을 열도록 한 문서를 가리킴
- window.parent▶ 상위 프레임을 가리킴
- window.self▶ 현재 작업중인창
- window.top▶ 프레임이 설정되기 전에 상태로 돌아감
- window.classes▶ 문서 안에 정의된 모든 스타일시트의 정보를 갖음
- window.tags▶ 모든 태그의 정보를 나타냄
- window.screenX▶ 창의 x좌표 반환
- window.screenY▶ 창의 y좌표 반환
- window.close▶ 창이 닿여 있는지 확인 후 true, false 반환
- windwo.length▶ 창 안에 프레임 수 반환

----------윈도우 메소드-----------

- window.alert("메시지")▶ 경고 창
- window.prompt("메시지", "기본문구")▶ 입력 창 띄움
- window.confirm("메시지")▶ 확인, 취소창 띄움
- window.status="환영합니다."▶ 상태표시줄 표시
- window.close()▶ 창닫기
- window.moveBy(x,y)▶ 브라우저를 상태좌표로 지정한 픽셀만큼 이동
- window.moveTo(x,y)▶ 브라우저를 절대좌표로 지정한 픽셀만큼 이동
- window.resizeBy(x,y)▶ 브라우저의 크기를 상대적으로 지정한 픽셀만큼 설정
- window.resizeTo(x,y)▶ 브라우저의 크기를 절대 값으로 지정한 픽셀만큼 설정
- window.scroll(x,y)▶ 창이나 프레임 안의 내용을 스크롤함
- window.scrollBy(x,y)▶ 스크롤을 상대좌표로 이동
- window.scrollTo(x,y)▶ 스크롤을 절대좌표로 이동
- window.setTimeout("명령문",시간간격)▶ 일정한 시간 간격으로 명령문을 반복 실행(1/1000초 단위)
- window.clearTimout()▶ SetTimeout()으로 동작되는 타이머 해제
- window.print()▶ 현재 문서 출력
- window.back()▶ 한단계 이전 URL로 이동
- window.forward()▶ 한단계 이후 URL로 이동
- window.home()▶ 브라우저에서 home으로 지정된 URL로 이동
- window.stop()▶ 불러오기 중지
- window.find("문자열")▶ 지정된 문자열이 있는지 검사(true, false 값)
- window.open("경로","창이름","속성")▶ 새 창을 연다.


## 페이지 로드시 자동 sysdate 보여주기
```
window.onload = function() 
{
  document.getElementsByName('rcv_d')[0].value = new Date().toISOString().substring(0, 10);
}
```
ex) 2021-08-13
