# Conditional statements in C++

### References:
- https://www.geeksforgeeks.org/decision-making-c-c-else-nested-else/

### Questions:
###### 1. What's the output?

```cpp
int main()
{
    int a = 14, b = 67;

    if (a + b - 55 > 10)
        cout << "Hello";
    
    cout << "World";
    
    return 0;
}
```

- A: `World`
- B: `HelloWorld`
- C: `World`
- D: `None of the above`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

Since, `a = 14` and `b = 67`. So, `a + b - 55 = 14 + 67 - 55 = 26 > 10`. So, the required condition is `true` and hence, the `if` block will be executed. So, the final output will be `HelloWorld`.
</p>
</details>

---

###### 2. What's the output?

```javascript
for (var i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}

for (let i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}
```

- A: `0 1 2` and `0 1 2`
- B: `0 1 2` and `3 3 3`
- C: `3 3 3` and `0 1 2`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

Because of the event queue in JavaScript, the `setTimeout` callback function is called _after_ the loop has been executed. Since the variable `i` in the first loop was declared using the `var` keyword, this value was global. During the loop, we incremented the value of `i` by `1` each time, using the unary operator `++`. By the time the `setTimeout` callback function was invoked, `i` was equal to `3` in the first example.

In the second loop, the variable `i` was declared using the `let` keyword: variables declared with the `let` (and `const`) keyword are block-scoped (a block is anything between `{ }`). During each iteration, `i` will have a new value, and each value is scoped inside the loop.

</p>
</details>

---



### TODO
- [ ] Add important questions
- [ ] Add more programs
- [ ] Add more links
