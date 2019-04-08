# Python Import Problem

## 問題

a.py

```python
def _print_abc():
    print("abc")
def print_something():
    _print_abc()
```

b.py

```python
from a import print_something

print_something()
```

為什麼我們只 import a 的 `print_something` ，但是 `_print_abc` 會被執行，而不是 `_print_abc`  not define

## 解決

來源： PTT 發問

因為 from 已經把 a.py 的程式碼讀過後，在給予 `print_something`