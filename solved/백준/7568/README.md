### 백준  - [7568](https://www.acmicpc.net/problem/7568)

### 풀이

* 대부분의 풀이가 비슷.

```Python
info = [list(map(int, input().split())) for _ in range(int(input()))]

rank = []

for i in range(len(info)):
    val = 1
    for k in range(len(info)):
        if info[i][0] < info[k][0] and info[i][1] < info[k][1]:
            val += 1
    rank.append(val)

print(' '.join(list(map(str, rank))))
```

