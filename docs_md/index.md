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
      append(str(args[-1]))
    append(end)
    if flush:
      cls.flush()

  @classmethod
  def flush(cls) -> None:
    os.write(1, cls.sb.build().encode())
    cls.sb = StringBuilder()

write = FastO.write
flush = FastO.flush

import sys
import math
import random
from bisect import bisect_right, bisect_left
from itertools import product, permutations, combinations, combinations_with_replacement 
from collections import deque, defaultdict, Counter
from heapq import heapify, heappush, heappop
from functools import lru_cache, reduce
INF = float('inf')
def error(*args, sep=' ', end='\n'):
  print(*args, sep=sep, end=end, file=sys.stderr)

# mod = 1000000007
# mod = 998244353

# dx = [-1, 0, 0, 1]
# dy = [0, -1, 1, 0]

# dx = [-1, -1, -1, 0, 0, 1, 1, 1]
# dy = [-1, 0, 1, -1, 1, -1, 0, 1]

sys.setrecursionlimit(7*10**5)
input = lambda: sys.stdin.readline().rstrip()
# input = lambda: sys.stdin.buffer.readline().rstrip()
```

