# TypeScript

## what is typescript?

TypeScript는 컴파일하면 JavaScript가 되는(compile-to-JavaScript) 언어이며,
컴파일 시점에 타입 체크를 하고, 전통적인 객체기반 프로그래밍 패턴을 도입하는 것 이외에도 강력한 기능들을 JavaScript 에 추가한다.

### 비슷한 다른 javascript의 변환 언어들

- CoffeeScript = tataly different with javascripy
- TypeScript = javascript + a = just added function, no strict
- ClojureScript
- GorillaScript
- Dart = between coffee and java

## Advance of Typescript

- additional functions
  - 인터페이스와 추상 클래스
  - 대수(algebraic) 데이터 타입
  - 다른 라이브러리들을 추가적으로 사용할 필요 X

![flow](https://cdn-images-1.medium.com/max/800/1*IP44ejhk2c78Nt_xUckWbw.png)

## Install typeScript

basic environment : npm, VScode or editor, package.json

### install typeScript by console

```
npm install --save-dev typescript
```

or

```
npm install --global typescript
```

### install React or Preact

```
npm install react react-dom
```

```
npm install --save-dev @types/react @types/react-dom
```

### install typescript compiler

```
npm init
tsc — init
```

## type of typeScript

- boolean

```
let isDone: boolean = false;

```

- numbers

```
let decimal: number = 6;
let hex: number = 0xf00d;
let binary: number = 0b1010;
let octal: number = 0o744;
```

- string

```
let name: string = "Jayson";
name = 'Allen';
```

- Object

```
declare function create(o: object | null): void;

create({ prop: 0 }); // OK
create(null); // OK

create(42); // Error
create("string"); // Error
create(false); // Error
create(undefined); // Error

```

- Array

```
// if array elements are Number
let list: number[] = [1, 2, 3];

// if array element is String
let list:
```

- Tuple

```
// array which contain Number and String both
let x: [string, number]; // type order must be correct
```

- Enum

```
enum Color {Red, Green, Blue}
let c: Color = Color.Green;
```

- Any

```
// can be inserted any types
let notSure: any = 4;
notSure = "maybe a string instead";
notSure = false;
```

- Void

```
// similar with Any but it has no return type
function warnUser(): void {
    console.log("This is my warning message");
}
```

- Null and Undefined

```
// 시작은 null, undefined 이지만 void, any처럼 어떤 값도 들어 갈 수 있다.
// `--strictNullChecks` 와 함깨 쓰면 개꿀
// Not much else we can assign to these variables!
let u: undefined = undefined;
let n: null = null;
```

- Never

```
// 별게 다 있음...
// Function returning never must have unreachable end point
function error(message: string): never {
    throw new Error(message);
}

// Inferred return type is never
function fail() {
    return error("Something failed");
}

// Function returning never must have unreachable end point
function infiniteLoop(): never {
    while (true) {
    }
}

```

## typescript usage

- typescript 파일 형식 : \*.ts
- tsc fileName : javascript로 파일 변환 (default ES3)
- tsc fileName -t es6 : 특정 옵션으로 변환 ( 예: ES6 )
- 변환시 확장자명 생략 가능, 여러개 동시 변환 가능 (ex. tsc fileOne fileTwo \*.ts)
- tsc fileName --watch : 변경사항 자동 감지 및 변환
- 변수 대입 : 백틱 안에 변수 대입 (ex. `${variable}`)
- example.code

```
function sum(a: number, b: number) {
  return a + b;
}

sum('x', 'y');
```

```
// person.ts
class Person {
  private name: string;

  constructor(name: string) {
    this.name = name;
  }

  sayHello() {
    return "Hello, " + this.name;
  }
}

const person = new Person('Lee');

console.log(person.sayHello());
```
