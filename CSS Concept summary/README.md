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
#### block
- 기본적으로 너비 100%(width:100%)속성을 가지고 있다.
- enter 키를 누르지 않았는데도 줄바꿈을 한 효과를 가지고 있다.
<img width="80%" src="https://user-images.githubusercontent.com/83212040/125604686-0c7b6184-f9d6-4349-bda5-46fc9a07fbc5.png"/>

#### inline
- 컨텐츠를 딱 감쌀정도의 크기만 갖게된다. 
- block태그와 다르게 줄바꿈이 되지 않고, 반드시 컨텐츠를 감싸게 되고, 크기를 변화시킬 수 없다.
<img width="8%" src="https://user-images.githubusercontent.com/83212040/125604981-6232abe1-e912-4203-b22d-39fa9846407c.png"/>

#### inline-block
- inline과 block의 특성을 합쳐놓은 속성이다. 
- 기본적으로는 inline의 속성을 지니고 있지만, 임의로 크기를 바꿔줄 수 있다.
<img width="40%" src="https://user-images.githubusercontent.com/83212040/125605033-73d898ec-da43-430a-a8e4-d7a78526e8d6.png"/>
