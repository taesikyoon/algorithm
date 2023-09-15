[코딩테스트 연습 - JadenCase 문자열 만들기](https://school.programmers.co.kr/learn/courses/30/lessons/12951)

```tsx
function solution(s) {
    let JadenCase = s.split(' ');
    
    for (let i = 0; i < JadenCase.length; i++) {
        if (!JadenCase[i][0]) continue;
        const firstWord = JadenCase[i][0].toUpperCase()
        const lowerString = JadenCase[i].slice(1).toLowerCase()
        JadenCase[i] =  firstWord + lowerString
    }
    return JadenCase.join(' ');
}
```