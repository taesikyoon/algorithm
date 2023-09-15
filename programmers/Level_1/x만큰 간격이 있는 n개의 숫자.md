[코딩테스트 연습 - x만큼 간격이 있는 n개의 숫자](https://school.programmers.co.kr/learn/courses/30/lessons/12954)

### 문제 풀이 코드

```jsx
function solution(x, n) {
    var answer = [];
    for (let i = 1 ; i <= n; i++) answer.push(i*x)
    return answer;
}
```