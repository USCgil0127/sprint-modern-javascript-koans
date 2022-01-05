# Modern JavaScript Koans

이번 Sprint는 앞서 익힌 JavaScript를 Koans의 형태로 익히는 시간입니다. 화살표 함수나, 구조 분해 할당과 같은 최근에 주로 쓰이는 문법을 익힐 수 있는 기회입니다. 이와 함께 Modern JavaScript Koans를 통해 this 및 call, apply 등의 함수 메소드를 익힐 수 있습니다.

## Before You Learn
- package.json 에 포함되어 있는 npm script를 실행하는 방법을 이해하고 있어야 합니다.

## Getting Started
진행 방법은 앞서 진행했던 JavaScript Koans와 동일합니다. 다만 이번 시간은 KoansRunner가 html 파일로 존재하는 이전과 다르게, 테스트 실행이 npm script로 존재합니다. 그러므로 실행을 위해 다음 과정을 거쳐야 합니다.

[repository 주소](https://github.com/codestates/im-sprint-modern-javascript-koans)

- `[Lesson - node.js와 관련 도구]`에서 안내한 대로, nvm을 이용해 node.js를 설치해야 합니다.
- repository를 클론하여, 디렉토리를 살펴봅니다.
- repository를 클론한 곳에서 npm install을 이용해 dependency를 설치해야 합니다.
- package.json를 열어 여러가지 실행 가능한 스크립트를 확인합니다.
  - npm run test 를 이용해 koans를 테스트할 수 있습니다.
- modern-js-koans 디렉토리 안에 있는 테스트 케이스를 하나씩 통과합니다.

## Bare minimum requirements
다음 네가지의 테스트 스위트(test suite)를 통과하세요.

- AboutArrowFunction
- AboutDestructing
- AboutThis
- AboutFunctionMethods

[내가 정리한 화살표 함수와 this](https://velog.io/@gil0127/JS-%ED%99%94%EC%82%B4%ED%91%9C-%ED%95%A8%EC%88%98)

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

## 해당 [github 링크](https://github.com/USCgil0127/sprint-modern-javascript-koans)


