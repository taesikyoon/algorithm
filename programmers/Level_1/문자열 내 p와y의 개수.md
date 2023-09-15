[코딩테스트 연습 - 문자열 내 p와 y의 개수](https://school.programmers.co.kr/learn/courses/30/lessons/12916)

### 문제 풀이 코드

```jsx
function solution(s){
    let answer = 0;
    let str = s.toUpperCase()
   for(let i = 0 ; i <str.length;i++) {
       if (str[i] === "P") answer++
       if (str[i] === "Y") answer--
   }
    
    return !answer;
}
```