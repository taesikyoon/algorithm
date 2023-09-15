[코딩테스트 연습 - K번째수](https://school.programmers.co.kr/learn/courses/30/lessons/42748)

### 문제 풀이 코드

```jsx
function solution(array, commands) {
  var answer = [];
  let result = [];
  for (let i = 0; i < commands.length; i++) {
    answer[i] = array.slice(commands[i][0] - 1, commands[i][1]).sort((a, b) => {
      return a - b;
    });
    result[i] = answer[i][commands[i][2] - 1];
  }

  return result;
}
```