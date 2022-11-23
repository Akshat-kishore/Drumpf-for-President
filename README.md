# Drumpf-for-President
t = int(input())

for i in range(t):
    n, k = map(int,input().split())
    l = list(map(int,input().split()))
    c = 0
    s = []
    for j in range(n):
        if l[l[j] - 1] != l[j]:
            if l[j] not in s:
                if k <= l.count(l[j]):
                    c += 1
        s.append(l[j])
    print(c)
