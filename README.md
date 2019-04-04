# Learn TDD

> 참조: <https://github.com/dwyl/learn-tdd>

### 소프트웨어 테스트란?

소프트웨어 테스트는 주어진 입력과 예상 출력 간의 차이를 탐지하기 위해 소프트웨어 항목을 평가하는 프로세스이다. 테스트는 제품의 품질을 평가한다. 소프트웨어 테스팅은 개발 프로세스 중에 수행되어야하는 프로세스. 즉, 소프트웨어 테스팅은 검증 및 검증 프로세스이다.

### TDD란?

TDD (Test-Driven Development)는 테스트 및 리팩토링을 수행하기에 충분한 프로덕션 코드를 작성하기 전에 테스트를 작성하는 것. 즉, 기능 코드를 작성하기 전에 요구 사항이나 디자인을 생각하는 한 가지 방법.

### RED, GREEN, REFACTOR

1. 실패하는 테스트 작성  - (사용자) 요구 사항, 스토리를 이해하고 기대하는 것에 대한 테스트를 작성한다. (테스트가 처음에 실패하므로 'Red'가 된다.) 
2. 실패한 테스트가 통과하도록 만든다  - 기존의 테스트가 모두 통과하는지 확인하면서 실패한 테스트가 통과하기 위한 코드를 작성한다. 
3. 작성한 코드를 리팩터링 - 만약에 현재 기능을 제공하기 전에 (사용자나 동료가 이해할 수 있도록)코드를 정리할 시간이 있다면  (사용자나 동료가 이해할 수 있도록) 더 간단하게 작성한다. 

### 테스트 작성

```javascript
 test('This is what a failing test looks like!', function(assert) {
        var result = [1,2,3].indexOf(1);  // this should be 0
        assert.equal(result, -1); // we *expect* this to fail
      });
```

1. Description - 보통 QUnit의 test () 메소드의 첫 번째 매개 변수
2. Computation - 함수 / 메소드 실행 (테스트 해결을 위해 작성하는 메소드 실행)
3. Assertion - 계산 결과가 예상 한 결과인지 확인

