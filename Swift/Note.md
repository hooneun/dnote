
### Variables

```swift
var greeting = "Hello, World"
greeting = "Hello, Swift" // (O))
```

### Constants

```swift
let greeting = "Hello, World" 
greeting = "Hello, Swift" // (X)
```

### String

```swift
let reuslt = "Ok!"

let quote = "hi, \"Swift\""

let greeting = "Hello,
I am Swift" // (X)

let greeting = """
Hello,
I'm Swift!
""" // (O)

let gretting = "Hello"
print(greeting.count) // 5
print(greeting.uppercased()) // HELLO
print(greeting.hasPrefix("H")) // true
print(greeting.hasPrefix("B")) // false
print(greeting.hasSuffix("ello")) // true
print(greeting.hasSuffix("bye")) // false

let hello = "안녕하세요"
print(hello.count) // 5
print(hello.uppercased()) // 안녕하세요

let hello = "Hello, "
let world = "world!"
let greeting = hello + world
print(greeting) // Hello, World!

let name = "Swift"
let age = 5
let message = "Hello, I'm \(name) and \(age) years old."
print("5 x 5 = \(5 * 5)") // 5 x 5 = 25
```

### Int
```swift
let score = 10

let lowerScore = score - 2
let higherScore = score + 10
let doubledScore = score * 2

var counter = 5
counter += 5
counter *= 2
counter -= 10
counter /= 2

let overTime = 10000 // 10000
let overTime = 10_000 // 10000
let overTime = 10_00____0 // 10000

let number = 120
print(number.isMultiple(of: 3)) // true 3의 배수 확인
```

### Double
```swift
let number = 0.1
let number2 = 0.2

print(number + number2) // 0.30000000000000004

let a = 1
let b = 1.0
print(a + b) // err, Swift는 Int와 Double를 다른 타입이라 생각한다.
```


### Boolean
```swift
let bool1 = true
let bool2 = false

bool1.toggle() // false
```


### Array
```swift
var numbers = [1, 2, 3, 4, 5]
print(numbers[0]) // 1
print(numbers[1]) // 2
numbers.append(6)
print(numbers) // [1, 2, 3, 4, 5, 6]
print(numbers.count) // 6
print(numbers.contains(6)) // true
print(numbers.sorted()) // 정렬
print(numbers.reversed()) // 역순 정렬

let numbers2 = [4, 5, 6, 7]
print(numbers + numbers2) // [1, 2, 3, 4, 5, 6, 7]

```

### Dictionary
```swift
let languages = [
    "Swift": "Apple",
    "Java": "Oracle",
    "Kotlin": "JetBrains"
]
  
print(languages["Swift"]) // Optional("Apple")
print(languages["Swift", default: "Unknown"]) // "Apple"

let languages = [String: String]()
languages["Swift"] = "Apple"
```

### Set
```swift
// 중복 항목 추가 X, 항목을 순서대로 저장하지 않음
// insert(), contains()...
var languages = Set(["Swift", "Rust", "Go", "PHP"])
print(languages) // ["Rust", "PHP", "Swift", "Go"]
languages.insert("Javascript") // ["Rust", "PHP", "Swift", "Go", "Javascript"]
print(languages)
```

### Operators
```swift
let firstNumber = 10
let secondNumber = 2

let sum = firstNumber + secondNumber // 12 더하기
let sub = firstNumber - secondNumber // 8 빼기

let mul = firstNumber * secondNumber // 20 곱하기
let div = firstNumber / secondNumber // 5 나누기
let remain = 13 & firstNumber // 3 나머지

let firstArr = ["A", "B"]
let secondArr = ["C", "D"]
print(firstArr + secondArr) // ["A", "B", "C", "D"]

var num = 100
num -= 5
print(num) // 95

var desc = "Hello"
desc += " World"
print(desc) // Hello World
```
