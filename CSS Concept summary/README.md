<div align="center" id="top">
<img height="270px" width="270px" src="./logo.png"><br>
  <h1>📃개념 및 궁금증 정리</h1>
</div>

***

## !important
* CSS는 같은 속성을 여러 번 정의했을 때, 나중에 설정한 값이 적용된다.
* 나중에 설정한 값이 적용되지 않게 하려면 속성값 뒤에 !important를 붙입니다.
```
p {
  color: red !important;  <-- red로 적용
}
p {
  color: blue;
}
```

## display 속성
block
- 기본적으로 너비 100%(width:100%)속성을 가지고 있다.
- enter 키를 누르지 않았는데도 줄바꿈을 한 효과를 가지고 있다.
