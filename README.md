# Modern JavaScript Koans

이번 Sprint는 앞서 익힌 JavaScript를 Koans의 형태로 익히는 시간입니다. 화살표 함수나, 구조 분해 할당과 같은 최근에 주로 쓰이는 문법을 익힐 수 있는 기회입니다. 이와 함께 Modern JavaScript Koans를 통해 this 및 call, apply 등의 함수 메소드를 익힐 수 있습니다.

## Before You Learn
- package.json 에 포함되어 있는 npm script를 실행하는 방법을 이해하고 있어야 합니다.

## Bare minimum requirements
다음 네가지의 테스트 스위트(test suite)를 통과하세요.

- AboutArrowFunction
- AboutDestructing
- AboutThis
- AboutFunctionMethods

[내가 정리한 this](https://velog.io/@gil0127/JS-this)

[내가 정리한 화살표 함수와 this](https://velog.io/@gil0127/JS-%ED%99%94%EC%82%B4%ED%91%9C-%ED%95%A8%EC%88%98)

[내가 정리한 Spread operator와 Rest Parameter](https://velog.io/@gil0127/Inheritance-Patterns)

[내가 정리한 구조분해할당](https://velog.io/@gil0127/%EA%B5%AC%EC%A1%B0-%EB%B6%84%ED%95%B4-%ED%95%A0%EB%8B%B9-%EA%B0%9D%EC%B2%B4-%EB%B0%B0%EC%97%B4)

[내가 정리한 call, apply, bind](https://velog.io/@gil0127/call-apply-bind)


## Advanced Challenges
AboutFunctionMethods 에는 `xdescribe` 로 표시된 pending 테스트들이 존재합니다. 추가적으로 이 테스트까지도 통과하고 싶다면, `xdescribe`를 `describe`로 바꾸어 테스트 통과에 도전해보세요!

보다 깊게 JavaScript의 원리를 알아갈 수 있을 것입니다.

- AboutFunctionMethods
  - call, apply의 유용한 예제를 확인합니다
  - bind의 유용한 예제를 확인합니다
  
  
---------


## Sprint 진행 후, 느낀 점

특별히, 어려웠던 부분은 없었다. 그러나, 아무래도 손에 잘 안 익으면 잘 안 쓰게 되기 때문에, 다시 한 번 해당 개념들을 손에 익힐 수 있었고 다양한 응용방식을 확인할 수 있었다.

-  클로져를 이용해서 태그와 안에 내용물을 찍어내는 함수를 여러번 보게 되는데, 구지 이렇게 함수까지 만들어서 써야하는 이유를 모르겠다.
그냥 이렇게 클로져를 쓸수 있구나... 정도로 이해하고 넘어간다.

-  화살표 함수 사용시, `this` 사용을 조심하자!!

```js
 module.exports.value = 100

    const counter = {
      value: 0,
      increse: () => {
        this.value++
      },
      decrease: () => {
        this.value--
      },
      getValue: () => {
        return this.value
      }
    }

    counter.increse()
    counter.decrease()
    counter.decrease()
    expect(counter.getValue()).to.eql(99)

    // 메소드 선언시에는 화살표 함수를 사용을 피하거나,
    // 화살표 함수를 사용할 경우 this 사용을 피해야 한다
    // 화살표 함수는 고유의 this 값을 가지지 못하니까, 상위 스코프에서 this 값을 찾는구나

```
=> 알고 있었는데도, 실전에서는 헷갈렸다.

- `apply`는 스프레드 연산자가 나오면서, `apply`의 역할이 대체된 것같다.

- 이 3가지 메소드 중에서 `bind`가 가장 유용하고, 앞으로도 많이 쓰일 것같다. 그 다음은 `call`
