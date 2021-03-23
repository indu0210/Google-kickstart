import math
T = int(input())
for j in range (T):
    count = 0
    N, K = map(int, input().split())
    s = input()
    for i in range(math.ceil((N-1)/2)):
        if (s[i] != s[N-i-1]):
            count = count +1;
    print("Case #{}: {}".format(j+1, abs(K -count)))