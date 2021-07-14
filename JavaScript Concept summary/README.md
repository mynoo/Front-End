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
