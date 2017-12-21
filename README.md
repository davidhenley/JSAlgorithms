Javascript Algorithms / Interview Questions
===

String Reversal
---

Option 1:
```
function reverseString(str) (
  Array.from(str).reverse().join('')
)
```

Option 2:
```
function reverseString(str) (
  Array.from(str).reduce((a, b) => b + a, '')
)
```

Option 3:
```
const reverseString = str => {
  let reversed = ''

  for (let char of reversed) {
    reversed = char + reversed
  }

  return reversed
}
```

String Palindrome
---

```
const isPalindrome = str => {
  const rev = Array.from(str).reverse().join('')

  return rev === str
}
```

Reverse Integers
---

```
const reverseInt = num => {
  const rev = num.toString.split('').reverse().join('')

  return parseInt(rev) * Math.sign(num)
}
```

String Max Characters
---

```
const maxChars = str => {
  const chars = {}
  let max = 0, maxChar = ''

  for (let char of str) {
    chars[char] = chars[char] + 1 || 1
    if (chars[char] > max) {
      max = chars[char]
      maxChar = char
    }
  }

  return maxChar
}
```

FizzBuzz
---
```
const fizzBuzz = num => {
  if (num < 1) return

  for (let i = 1; i <= num; i++) {
    let str = ''
    if (i % 3 === 0) str += 'fizz'
    if (i % 5 === 0) str += 'buzz'
    console.log(str || i)
  }
}
```