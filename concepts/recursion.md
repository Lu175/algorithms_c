### Recursion 

* Factorial (순차 곱셈)
    * n 을 인자로 받는다. 
    * n 이 0보다 큰 경우 n * f(n-1) 을 반환한다. 
    * n 이 0 이 될 때 1을 반환한다. 
    
* 직접 재귀, 간접 재귀 
    * 함수 내부에서 자기 자신의 함수를 다시 호출하면 직접 재귀이다. 
    * 함수 a가 b 를 호출하고 다시 b 가 a를 호출하는 경우 간접 재귀이다. 
    
* 재귀 알고리즘에 알맞는 경우는 
    * 풀어야 할 문제
    * 계산할 함수 
    * 처리할 데이터 구조가 재귀로 정의되는 경우이다. 
    
* 유클리드 호제법 
    * 최대공약수를 재귀적으로 구하는 방법 (Greatest Common Divisor)
    * 직사각형을 정사각형으로 완전히 채운다. 
    * 이렇게 만들 수 있는 정사각형의 가장 긴 변의 길이를 구한다. 
    
``` 
x = a*z 와 y = b*z 를 만족시키는 최대의 정수 z가 존재할 때
z = gdc(x, y)  

최대 공약수는 y = 0 이면 x이고
y가 0이 아니면, gcd(y , x % y) 이다.  

```

### 재귀 알고리즘 분석 

* 하향식 분석과 상향식 분석 (top down & bottom up)

* 재귀 알고리즘의 분석 
    * 재귀 호출을 여러 회 실행하는 함수를 순수하게(genuinely) 재귀적이라 함. 

* [메모이제이션](https://ko.wikipedia.org/wiki/%EB%A9%94%EB%AA%A8%EC%9D%B4%EC%A0%9C%EC%9D%B4%EC%85%98)
    * 배열에 계산 결과를 저장, 위로 올라가면서 배열의 값을 가져다 씀. 

* [블로그 포스트: 꼬리 재귀 최적화(Tail Recursion)](https://bozeury.tistory.com/entry/%EA%BC%AC%EB%A6%AC-%EC%9E%AC%EA%B7%80-%EC%B5%9C%EC%A0%81%ED%99%94Tail-Recursion) 