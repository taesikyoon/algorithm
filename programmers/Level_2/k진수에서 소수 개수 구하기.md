[코딩테스트 연습 - k진수에서 소수 개수 구하기](https://school.programmers.co.kr/learn/courses/30/lessons/92335)

### 풀이 코드

```jsx
function solution(n, k) {
  var answer = 0;
  let changeNumber = n.toString(k).split("0");
  for (let i = 0; i < changeNumber.length; i++) {
    if (isPrime(changeNumber[i])) answer++;
  }
  return answer;
}

function isPrime(number) {
  if (number < 2) return false;
  for (let i = 2; i * i <= number; i++) {
    if (number % i == 0) return false;
  }
  return true;
}
```

풀이 과정

1. 소수를 판별하는 함수를 만들어준다.
2. k진수로 변경한 후 “0”을 기준으로 split 시켜준다.
3. 배열안에 함수들을 하나씩 소수 판별하며 소수면 answer++

- 2Level 치고 너무 쉽다.
