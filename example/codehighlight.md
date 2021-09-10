% Hello Code Highlight
% Your name
% October 7, 2020

# Code Highlighting

## Default

```
// This is a default code block.
function fib(n) {
    if (n < 3) return n;
    return fib(n-2) + fib(n-1);
}
```

## Console

```console
// This is a console block.
function fib(n) {
    if (n < 3) return n;
    return fib(n-2) + fib(n-1);
}
```

## Kinx

```kinx
// This is a kinx block.
function fib(n) {
    if (n < 3) return n;
    return fib(n-2) + fib(n-1);
}
System.println(fib(34));
```

## JavaScript

```javascript
// This is a javascript block.
function fib(n) {
    if (n < 3) return n;
    return fib(n-2) + fib(n-1);
}
console.log(fib(34))
```

<pagebreak />

## Ruby

```ruby
# This is a ruby block.
def fib(n)
  return n if n < 3
  fib(n-1) + fib(n-2)
end
p fib(34)
```

## Python

```python
# This is a python block.
def fib(n):
    if n < 3:
        return n
    else:
        return fib(n-1) + fib(n-2)
print fib(34)
```

## C

```c
/* This is a c block. */
#include <stdio.h>
int fib(int n) {
    if (n < 3) return n;
    return fib(n-2) + fib(n-1);
}
int main() {
    printf("%d", fib(34));
}
```

## C++

```cpp
/* This is a cpp or c++ block. */
#include <cstdio>
class fibonacci {
private:
    int calc(int n) {
        if (n < 3) return n;
        return calc(n-2) + calc(n-1);
    }
public:
    int operator()(int n) {
        return calc(n);
    }
};
int main() {
    fibonacci fib;
    printf("%d", fib(34));
}
```

## JSON

```json
{
    "fib": {
        "name": "fibonacci",
        "cond": [
            "if (n < 3) -> n",
            "otherwise, fib(n-2) + fib(n-1)"
        ]
    }
}
```

You can see the differences between code blocks.
