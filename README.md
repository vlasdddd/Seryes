# Series1
s = 0
for i in range(10):
    a = float(input())
    s = s + a
print(s)


# Series2
p = 1
for i in range(10):
    a = float(input())
    p = p * a
print(p)


# Series3
s = 0
for i in range(10):
    a = float(input())
    s = s + a
print(s / 10)


# Series4
n = int(input())
s = 0
p = 1
for i in range(n):
    a = float(input())
    s = s + a
    p = p * a
print(s)
print(p)


# Series5
n = int(input())
s = 0
for i in range(n):
    a = float(input())
    b = int(a)
    print(float(b))
    s = s + b
print(s)


# Series6
n = int(input())
p = 1
for i in range(n):
    a = float(input())
    b = a - int(a)
    print(b)
    p = p * b
print(p)


# Series7
n = int(input())
s = 0
for i in range(n):
    a = float(input())
    b = round(a)
    print(b)
    s = s + b
print(s)


# Series8
n = int(input())
k = 0
for i in range(n):
    a = int(input())
    if a % 2 == 0:
        print(a)
        k = k + 1
print(k)


# Series9
n = int(input())
k = 0
for i in range(n):
    a = int(input())
    if a % 2 != 0:
        print(i + 1)
        k = k + 1
print(k)


# Series10
n = int(input())
found = False
for i in range(n):
    a = int(input())
    if a > 0:
        found = True
if found:
    print("TRUE")
else:
    print("FALSE")


# Series11
k = int(input())
n = int(input())
found = False
for i in range(n):
    a = int(input())
    if a < k:
        found = True
if found:
    print("TRUE")
else:
    print("FALSE")


# Series12
k = 0
a = int(input())
while a != 0:
    k = k + 1
    a = int(input())
print(k)


# Series13
s = 0
a = int(input())
while a != 0:
    if a > 0 and a % 2 == 0:
        s = s + a
    a = int(input())
print(s)


# Series14
k = int(input())
count = 0
a = int(input())
while a != 0:
    if a < k:
        count = count + 1
    a = int(input())
print(count)


# Series15
k = int(input())
number = 0
answer = 0
a = int(input())
while a != 0:
    number = number + 1
    if a > k and answer == 0:
        answer = number
    a = int(input())
print(answer)


# Series16
k = int(input())
number = 0
answer = 0
a = int(input())
while a != 0:
    number = number + 1
    if a > k:
        answer = number
    a = int(input())
print(answer)


# Series17
b = float(input())
n = int(input())
inserted = False
for i in range(n):
    a = float(input())
    if a >= b and not inserted:
        print(b)
        inserted = True
    print(a)
if not inserted:
    print(b)


# Series18
n = int(input())
last = 0
for i in range(n):
    a = int(input())
    if i == 0 or a != last:
        print(a)
    last = a


# Series19
n = int(input())
a = int(input())
k = 0
for i in range(1, n):
    b = int(input())
    if b < a:
        print(b)
        k = k + 1
    a = b
print(k)


# Series20
n = int(input())
a = int(input())
k = 0
for i in range(1, n):
    b = int(input())
    if a < b:
        print(a)
        k = k + 1
    a = b
print(k)


# Series21
n = int(input())
a = float(input())
ok = True
for i in range(1, n):
    b = float(input())
    if b <= a:
        ok = False
    a = b
if ok:
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
        if not ((b > a and b > c) or (b < a and b < c)):
            answer = i - 1
    a = b
    b = c
print(answer)


# Series24
n = int(input())
a = []
for i in range(n):
    a.append(int(input()))

last = -1
second = -1

for i in range(n):
    if a[i] == 0:
        second = last
        last = i

s = 0

for i in range(second + 1, last):
    s = s + a[i]

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
    s = s + a[i]

print(s)


# Series26
k = int(input())
n = int(input())

for i in range(n):
    a = float(input())
    print(a ** k)


# Series27
n = int(input())

for i in range(1, n + 1):
    a = float(input())
    print(a ** i)


# Series28
n = int(input())

for i in range(1, n + 1):
    a = float(input())
    print(a ** (n - i + 1))


# Series29
k = int(input())
n = int(input())

s = 0

for i in range(k):
    for j in range(n):
        a = int(input())
        s = s + a

print(s)


# Series30
k = int(input())
n = int(input())

for i in range(k):
    s = 0

    for j in range(n):
        a = int(input())
        s = s + a

    print(s)


# Series31
k = int(input())
n = int(input())

count = 0

for i in range(k):
    found = False

    for j in range(n):
        a = int(input())

        if a == 2:
            found = True

    if found:
        count = count + 1

print(count)


# Series32
k = int(input())
n = int(input())

for i in range(k):
    answer = 0

    for j in range(n):
        a = int(input())

        if a == 2 and answer == 0:
            answer = j + 1

    print(answer)


# Series33
k = int(input())
n = int(input())

for i in range(k):
    answer = 0

    for j in range(n):
        a = int(input())

        if a == 2:
            answer = j + 1

    print(answer)


# Series34
k = int(input())
n = int(input())

for i in range(k):
    s = 0
    found = False

    for j in range(n):
        a = int(input())

        s = s + a

        if a == 2:
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
    a = int(input())

    while a != 0:
        count = count + 1
        total = total + 1
        a = int(input())

    print(count)

print(total)


# Series36
k = int(input())
answer = 0

for i in range(k):
    a = int(input())
    increasing = True

    b = int(input())

    while b != 0:
        if b <= a:
            increasing = False

        a = b
        b = int(input())

    if increasing:
        answer = answer + 1

print(answer)


# Series37
k = int(input())
answer = 0

for i in range(k):
    a = int(input())

    increasing = True
    decreasing = True

    b = int(input())

    while b != 0:
        if b <= a:
            increasing = False

        if b >= a:
            decreasing = False

        a = b
        b = int(input())

    if increasing or decreasing:
        answer = answer + 1

print(answer)


# Series38
k = int(input())

for i in range(k):
    a = int(input())

    increasing = True
    decreasing = True

    b = int(input())

    while b != 0:
        if b <= a:
            increasing = False

        if b >= a:
            decreasing = False

        a = b
        b = int(input())

    if increasing:
        print(1)
    elif decreasing:
        print(-1)
    else:
        print(0)


# Series39
k = int(input())
answer = 0

for i in range(k):
    a = int(input())
    b = int(input())

    zigzag = True

    c = int(input())

    while c != 0:
        if not ((b > a and b > c) or (b < a and b < c)):
            zigzag = False

        a = b
        b = c
        c = int(input())

    if zigzag:
        answer = answer + 1

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
        number = number + 1

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
