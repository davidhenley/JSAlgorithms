Javascript Algorithms / Interview Questions
===

String Reversal
---

Option 1:
```
const reverseString = str => (
  Array.from(str).reverse().join('')
)
```

Option 2:
```
const reverseString = str => (
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