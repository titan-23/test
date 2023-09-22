_____

# [test](https://github.com/titanium-22/test)

**2023/9/11 追記**

**注意！ライブラリ魔改造に伴って、色々壊れています！怖すぎ！**

[titan23](https://atcoder.jp/users/titan23) が使用している、競技プログラミング用のライブラリです。 PyPy で動きます。  
各 REAMDME はサボっています。また、ありえないバグを仕込んでたりします。ご注意ください。  
誰かがバグに引っかかって WA を出してくれたら、筆者冥利に尽きます。  

[使い方](HowToUse.md)

_____

## [Algorithm](Algorithm/Algorithm.md)

### [Mo](Algorithm/Mo/Mo.md)

```python
import os
from __pypy__.builders import StringBuilder

class FastO():

  sb = StringBuilder()

  @classmethod
  def write(cls, *args, sep: str=' ', end: str='\n', flush: bool=False) -> None:
    append = cls.sb.append
    for i in range(len(args)-1):
      append(str(args[i]))
      append(sep)
    if args:

```

