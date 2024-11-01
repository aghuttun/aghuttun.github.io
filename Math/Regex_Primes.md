# A regular expression to check for prime numbers

https://www.noulakaz.net/2007/03/18/a-regular-expression-to-check-for-prime-numbers/

https://www.youtube.com/watch?v=B9H0TyApBtU

```text
/^1?$|^(11+?)\1+$/
```

```python
import re

if __name__ == '__main__':
    n = 13
    check = not re.match(pattern=r"^.?$|^(..+?)\1+$", string="1" * n)
    print(f"{n} prime? {check}")
```

