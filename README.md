# Series1
s = 0

for i in range(10):
    x = float(input())
    s += x

print(s)


# Series2
p = 1

for i in range(10):
    x = float(input())
    p *= x

print(p)


# Series3
s = 0

for i in range(10):
    x = float(input())
    s += x

print(s / 10)


# Series4
n = int(input())

s = 0
p = 1

for i in range(n):
    x = float(input())
    s += x
    p *= x

print(s)
print(p)


# Series5
n = int(input())
s = 0

for i in range(n):
    x = float(input())
    x = int(x)

    print(float(x))
    s += x

print(s)


# Series6
n = int(input())
p = 1

for i in range(n):
    x = float(input())
    x = x - int(x)

    print(x)
    p *= x

print(p)


# Series7
n = int(input())
s = 0

for i in range(n):
    x = float(input())
    x = round(x)

    print(x)
    s += x

print(s)


# Series8
n = int(input())
k = 0

for i in range(n):
    x = int(input())

    if x % 2 == 0:
        print(x)
        k += 1

print(k)


# Series9
n = int(input())
k = 0

for i in range(n):
    x = int(input())

    if x % 2 != 0:
        print(i + 1)
        k += 1

print(k)


# Series10
n = int(input())
flag = False

for i in range(n):
    x = int(input())

    if x > 0:
        flag = True

if flag:
    print("TRUE")
else:
    print("FALSE")


# Series11
k = int(input())
n = int(input())

flag = False

for i in range(n):
    x = int(input())

    if x < k:
        flag = True

if flag:
    print("TRUE")
else:
    print("FALSE")


# Series12
k = 0
x = int(input())

while x != 0:
    k += 1
    x = int(input())

print(k)


# Series13
s = 0
x = int(input())

while x != 0:
    if x > 0 and x % 2 == 0:
        s += x

    x = int(input())

print(s)


# Series14
k = int(input())
count = 0

x = int(input())

while x != 0:
    if x < k:
        count += 1

    x = int(input())

print(count)


# Series15
k = int(input())
number = 0
answer = 0

x = int(input())

while x != 0:
    number += 1

    if x > k and answer == 0:
        answer = number

    x = int(input())

print(answer)


# Series16
k = int(input())
number = 0
answer = 0

x = int(input())

while x != 0:
    number += 1

    if x > k:
        answer = number

    x = int(input())

print(answer)


# Series17
b = float(input())
n = int(input())

added = False

for i in range(n):
    x = float(input())

    if x >= b and not added:
        print(b)
        added = True

    print(x)

if not added:
    print(b)


# Series18
n = int(input())
last = None

for i in range(n):
    x = int(input())

    if i == 0 or x != last:
        print(x)

    last = x


# Series19
n = int(input())

a = int(input())
count = 0

for i in range(n - 1):
    b = int(input())

    if b < a:
        print(b)
        count += 1

    a = b

print(count)


# Series20
n = int(input())

a = int(input())
count = 0

for i in range(n - 1):
    b = int(input())

    if a < b:
        print(a)
        count += 1

    a = b

print(count)


# Series21
n = int(input())
a = float(input())

flag = True

for i in range(n - 1):
    b = float(input())

    if b <= a:
        flag = False

    a = b

if flag:
    print("TRUE")
else:
    print("FALSE")


# Series22
n = int(input())
a = float(input())

answer = 0

for i in range(2, n + 1):
    b = float(input())

    if answer == 0 and b >= a:
        answer = i

    a = b

print(answer)


# Series23
n = int(input())

a = float(input())
b = float(input())

answer = 0

for i in range(3, n + 1):
    c = float(input())

    if answer == 0:
        if (b >= a and b <= c) or (b <= a and b >= c):
            answer = i - 1

    a = b
    b = c

print(answer)


# Series24
n = int(input())
a = []

for i in range(n):
    a.append(int(input()))

first = -1
second = -1

for i in range(n):
    if a[i] == 0:
        second = first
        first = i

s = 0

for i in range(second + 1, first):
    s += a[i]

print(s)


# Series25
n = int(input())
a = []

for i in range(n):
    a.append(int(input()))

first = -1
last = -1

for i in range(n):
    if a[i] == 0:
        if first == -1:
            first = i

        last = i

s = 0

for i in range(first + 1, last):
    s += a[i]

print(s)


# Series26
k = int(input())
n = int(input())

for i in range(n):
    x = float(input())
    print(x ** k)


# Series27
n = int(input())

for i in range(1, n + 1):
    x = float(input())
    print(x ** i)


# Series28
n = int(input())

for i in range(1, n + 1):
    x = float(input())
    print(x ** (n - i + 1))


# Series29
k = int(input())
n = int(input())

s = 0

for i in range(k):
    for j in range(n):
        x = int(input())
        s += x

print(s)


# Series30
k = int(input())
n = int(input())

for i in range(k):
    s = 0

    for j in range(n):
        x = int(input())
        s += x

    print(s)


# Series31
k = int(input())
n = int(input())

count = 0

for i in range(k):
    found = False

    for j in range(n):
        x = int(input())

        if x == 2:
            found = True

    if found:
        count += 1

print(count)


# Series32
k = int(input())
n = int(input())

for i in range(k):
    answer = 0

    for j in range(n):
        x = int(input())

        if x == 2 and answer == 0:
            answer = j + 1

    print(answer)


# Series33
k = int(input())
n = int(input())

for i in range(k):
    answer = 0

    for j in range(n):
        x = int(input())

        if x == 2:
            answer = j + 1

    print(answer)


# Series34
k = int(input())
n = int(input())

for i in range(k):
    s = 0
    found = False

    for j in range(n):
        x = int(input())
        s += x

        if x == 2:
            found = True

    if found:
        print(s)
    else:
        print(0)


# Series35
k = int(input())
total = 0

for i in range(k):
    count = 0
    x = int(input())

    while x != 0:
        count += 1
        total += 1
        x = int(input())

    print(count)

print(total)


# Series36
k = int(input())
answer = 0

for i in range(k):
    a = int(input())
    flag = True

    b = int(input())

    while b != 0:
        if b <= a:
            flag = False

        a = b
        b = int(input())

    if flag:
        answer += 1

print(answer)


# Series37
k = int(input())
answer = 0

for i in range(k):
    a = int(input())

    up = True
    down = True

    b = int(input())

    while b != 0:
        if b <= a:
            up = False

        if b >= a:
            down = False

        a = b
        b = int(input())

    if up or down:
        answer += 1

print(answer)


# Series38
k = int(input())

for i in range(k):
    a = int(input())

    up = True
    down = True

    b = int(input())

    while b != 0:
        if b <= a:
            up = False

        if b >= a:
            down = False

        a = b
        b = int(input())

    if up:
        print(1)
    elif down:
        print(-1)
    else:
        print(0)


# Series39
k = int(input())
answer = 0

for i in range(k):
    a = int(input())
    b = int(input())

    flag = True
    c = int(input())

    while c != 0:
        if not ((b > a and b > c) or (b < a and b < c)):
            flag = False

        a = b
        b = c
        c = int(input())

    if flag:
        answer += 1

print(answer)


# Series40
k = int(input())

for i in range(k):
    a = int(input())
    b = int(input())

    number = 2
    answer = 0

    c = int(input())

    while c != 0:
        number += 1

        if answer == 0:
            if not ((b > a and b > c) or (b < a and b < c)):
                answer = number - 1

        a = b
        b = c
        c = int(input())

    if answer == 0:
        print(number)
    else:
        print(answer)
