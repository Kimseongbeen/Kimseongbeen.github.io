---
layout: post
title: "Javascript 04.문자열과 숫자 "
discription: "chrome console을 이용한 공부. "
date: 2020-06-23 23:40:00 +0700
category: [javascript]
---

## Console 사용하기

### 이항 연산자(산술 연산자)란?

`해당 연산의 실행을 위해서 두 개의 값이나 변수가 필요한 연산자를 의미합니다.`

예를 들어서 
```
1+1  //더하기
>2

2-1  //빼기
>1

3*2  //곱하기
>6

6/2  //나누기
>3
```
 숫자라는 데이터 타입이 어떻게 다루어지고 숫자를 연산해서 어떤 결과를 만들어내는
 산술연산자 4개를 만들어 봤습니다.

### 문자열

문자열을 표현하자면 

`"안녕", '안녕'` 

이렇게 나타낼 수 있습니다.

그러면 주제인 Console을 사용해 봐야할텐데

문자열의 길이를 알고 싶을때 사용하는 도구가 있습니다.

javascript의 문자열 문법을 알고 싶으면 구글에다가 "javascript string"을 검색하고 

가장 위에있는 MOZILLA 사이트에 들어가서 문자열과 길이(length)가 같이있는 String.length에 들어가보면

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/length

```
const str = 'Life, the universe and everything. Answer:';

console.log(`${str} ${str.length}`);
// expected output: "Life, the universe and everything. Answer: 42"

```
이렇게 표현을 해놨는데 str라는 변수에 문자열을 대입하고 str.length를 사용하므로써

문자열의 길이가 42라는 답이 나오는걸 볼 수 있고

여기서 문자열 뒤에 .length를 붙히면 문자열의 길이를 알 수 있다라는 답이 나왔습니다.

<img src="https://i.imgur.com/cmRn6mR.png" title="length.png"/>

그러면 관련 주제에 몇개를 더찾아보면

JavaScript Demo: String.toUpperCase()이라는 포스트가 있습니다.
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/toUpperCase

들어가서 보면 소문자를 대문자로 바꿔주는 역할을 하는 것을 볼 수 있습니다.
```
const sentence = 'The quick brown fox jumps over the lazy dog.';

console.log(sentence.toUpperCase());
// expected output: "THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG."

```

소문자가 들어가있는 문자열 뒤에 .toUpperCase()를 사용하면 문자열 안에 있는 소문자들이 대문자로 바뀝니다.

<img src="https://i.imgur.com/oy8Uq4F.png" title="toUpperCase.png"/>

다음 indexOf라는 것을 알아볼건데
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf

### Syntax(구문,의미)
`str.indexOf(searchValue[, fromIndex])`

의미를 보면 (searchValue)어떤 값을 찾는뜻입니다.

예문을 보면 원하는 값(숫자,문자열이지만 여기서는 문자열)이 몇번째 문자열에 나오는걸 보여주는데

직접 세보니 숫자가 -1되어서 나오는걸 알수 있는데 이유는

문자열의 첫번째 값은 1이아닌 0이라서 4번째에 나온다고하면 indexOf의 값은 3이 출력 되는것입니다.

<img src="https://i.imgur.com/GXkqStE.png" title="indexOf.png"/>
* 1부터가 아닌 0부터 세면 맞는것이 보입니다.

마지막으로 str문법을 끝내고

문자열과 숫자로 돌아오면

<img src="https://i.imgur.com/qICBzjh.png" title="숫자,문자열차이.png"/>

위 그림에서 보듯이 

1+1은 2라는 값이 나오지만

"1"+"1"은 "2"가아닌 "11"이 나오는걸 알 수 있습니다.

즉 ""안에 포함된 것은 숫자를 넣어도 문자열로 인식한다는것과 비슷해 보이지만 

문자열과 숫자의 연산 결과는 엄청나게 달라집니다.








