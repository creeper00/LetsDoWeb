# React - 1강

## React 출력하기
- [JSX 란 & 기본 ](https://reactjs.org/docs/introducing-jsx.html)   
    
    
JSX란 간단히 말해 JS + XML로 JS에서 확장한 문법 체계입니다. 여기서 XML은 HTML의 한계를 보완하기 위한 마크업언어입니다.  
JSX대해서는 간단히 알아두면 좋고, 앞으로 REACT를 배워가면서 천천히 체험해봐도 됩니다.   

일단 **CODEPEN** 으로 REACT의 기본을 연습해보면 좋을 것 같아요.
``` 
function formatName(user) {
  return user.firstName + ' ' + user.lastName;
}

const name = {
  firstName: 'Tony',
  lastName: 'Stark'
};

const element = (
  <h1>
    Hello, {formatName(name)}!
  </h1>
);

ReactDOM.render(
  element,
  document.getElementById('root')
);
```
위 코드에서 일단 눈에 띄는 3개는 function, const, render 겠죠?   
밑에 참조로 원본 문서를 달아놓았지만, 영어가 싫다거나 설명 스타일이 잘 안맞을 수 있어서 제 나름대로 정리해봤습니다.   
   
   
function은 다들 아는 함수에용. 변수(user)를 받아서 변수 속 firstname +' '(띄어쓰기)+ lastnam 을 붙여서 반환합니다.  
java랑 비슷하죠?   
다음으로 const는 이전 js에서 했던 immutable variable, 상수입니다.  
상수로 데이터 타입을 선언하고, 그 안에 firstname, lastname을 정의해놓았죠.  
불러올 땐 .firstname 이런식으로 사용합니다.   
JS에서 {}, 중괄호 안에는 올바른 JS expression은 다 들어갈 수 있습니다.
name 안에 object를 선언할 수도, function도 들어갈 수 있죠.  
element 에는 <> </> brace가 있죠? html에서 보셨을 텐데, 이 경우 중괄호를 쳐주면 error 가 뜹니다. ㅠㅠ   
<>brace와 겹치기 때문이죠.  
    
ReactDOM.reander는 보이는대로 '출력'을 담당합니다.   
가운데 element가 보이죠? element는 출력을 할수 있는 <> 가 존재해서 자동으로 출력이됩니다.
다른 식으로 출력하고 싶을 땐 직접 render 안에 {formatName(name)}을 적어줍시다. ( {}안에 함수를 넣으세요! 안넣으면... 직접 해보세요 )   
