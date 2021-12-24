# sprint-underbar

이전에는 배열 메소드가 브라우저에서 자체적으로 지원되지 않던 시절이 있었습니다. 보다 나은 방법으로 배열이나 객체를 다루기 위해 라이브러리, 즉 배열이나 객체를 다루기 위한 도구 모음집을 만들었습니다. 이번 스프린트 우리가 배열, 객체를 다루는 라이브러리 Underbar를 구현하며 자바스크립트 문법과 기본 알고리즘 구현에 대해서 자세히 배웁니다. 여러분이 이 라이브러리를 직접 만들어보면서 배열 메소드의 작동원리를 보다 더 심도있게 이해할 수 있습니다.

Underbar의 모티브가 되는 라이브러리로는, [underscore.js](https://underscorejs.org/), [lodash](https://lodash.com/)가 있습니다. 이 라이브러리는 여전히 JavaScript 생태계에서 많이 쓰이는 인기있는 라이브러리입니다. 여러분들도 보다 나은 프로그래밍을 해주는 라이브러리를 만들어서 효율적이고 아름다운 프로그래밍으로 한 발자국 더 나아가봅시다.

### Before You Learn
- 자바스크립트 배열 내장 메소드(forEach, map, filter, reduce 등)의 원리를 이해합니다.
- 코플릿 고차함수 01번 - 06번 문제를 복습하여 고차함수 기본 용법을 이해합니다.
- callback 함수를 전달하여 사용할 수 있습니다.
- closure 함수를 리턴하여 활용할 수 있습니다.
- `... (rest parameter)`를 사용하여 인자의 개수를 알 수 있고, 각 인자에 접근할 수 있어야 합니다.

### Achievement Goals

#### Part 1
- 많이 사용되는 기본적인 자바스크립트 배열 내장 메소드를 직접 구현하며 원리를 이해한다.
   - slice, forEach, indexOf, filter, map, reduce ...
- Higher Order Function을 활용하여 기존에 만든 함수를 callback으로 재사용 할 수 있다.
- iteratee가callback 함수임을 이해할 수 있다.
- callback 함수명을 기반으로 [사람이 읽기 쉬운 코드](https://ko.wikipedia.org/wiki/%EC%84%A0%EC%96%B8%ED%98%95_%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D)를 짤 수 있다.

#### Part 2
- Part 1에서 제작한 언더바 (`_`) 고차함수를 응용하여 Part 2를 해결할 수 있다.
   - 배열 내장 메소드 : includes, every, some
   - 객체 커스텀 메소드 : extends, defaults
   - 배열 커스텀 메소드 : zip, zipStrict, intersection, difference,, shuffle
- `rest parameter`를 자유자재로 사용할 수 있다.
- `_.shffule`에서 immutable 개념을 복습할 수 있다.

#### Getting Started

spec 디렉토리 안에 test suites 파일이 있습니다. 이 디렉토리의 모든 테스트를 통과시키는것이 목표입니다. 브라우저에서 SpecRunner.html을 열어 모든 테스트를 확인하세요. 테스트는 수정하실 필요가 없습니다!

src 디렉토리 안의 파일에는 함수에 대한 정의 및 설명이 들어 있습니다. 파일 내의 안내를 잘 읽고 따라와주시기 바랍니다. 유심히 읽어보시면, 각 함수의 body가 비어있는 것을 확인하실 수 있습니다. 여기를 체워주시고, SpecRunner.html에서 각 함수에 해당하는 테스트를 확인하면서 풀어주시면 됩니다.

### Bare Minimum Requirements

- Part 1(`src/01_part1.js`)파일을 수정하여, 테스트를 통과합니다.
- Part 2(`src/02_part2.js`)파일을 수정하여, 테스트를 통과합니다.

### 주의 사항 (Precautions)
- 이번 과제에서 극히 일부를 제외한 자바스크립트 배열 내장 메소드는 사용이 금지되어 있습니다. 자신이 만든 함수를 활용하여 함수 위주로 코드를 작성해봅시다.

- src 폴더에 있는 함수를 완성하시고, specRunner.html 를 열어서 src 폴더 내 파일에 작성되어 있는 함수가 통과되었는지 아닌지 확인하는 방식입니다. spec 디렉토리의 테스트는 수정하지 않아야 합니다 !

- 과제 제출 시, console.log를 제거합시다. console.log는 디버깅 목적으로 코드의 내부 작동 방식 파악에 도움이 되지만, 배포하는 코드는 외부인이 내부 작동 방식을 파악할 수 없어야 합니다. 해킹의 우려가 있을 수 있겠죠 :)

### Advanced Challenge
- 03_advanced.js를 수정하여 Advanced Test를 통과합니다.
   - SpecRunner.html을 실행했는데, Advanced Test가 보이지 않나요? 파일을 잘 살펴보시고 주석을 제거하세요 :)
- 여러분이 구현한 코드를 [실제 라이브러리](https://underscorejs.org/docs/underscore-esm.html)와 배포 될 레퍼런스와 비교하고, 더 나온 코드를 작성하기 위해 노력합니다. 이런 과정을 [리펙토링](https://en.wikipedia.org/wiki/Code_refactoring)이라고 합니다.

----------

### Sprint를 끝마치고 느낀점
reduce함수를 구현하는 것이 상당히 어려웠습니다. 그리고 Advanced Challenge 파트를 구현하는데, 상당히 시간을 들였지만, 결국 구현에 성공할 수 있었습니다.
