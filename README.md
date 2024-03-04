# slicing
# approach1 from starting
b = "Hello, World!"
print(b[:5])
# approach2 slice to end
b = "Hello, World!"
print(b[2:])
# approach3 negative index
b = "Hello, World!"
print(b[-5:-2])

# approach4
s=input()
x=s[::2]
print(len(x))'''


# approach5 using lists
s=input()
x=[]
for i in range(len(s)):
  if i%2==0:
    x.append(s[i])
y=[]
for i in range(len(s)):
  if i%2!=0:
    y.append(s[i])
x.extend(y)
print(*x,sep="")'''

# approach6
s=input()
x=""
y=""
for i in range(len(s)):
  if i%2==0:
    x=x+s[i]
for i in range(len(s)):
  if i%2!=0:
    y=y+s[i]
print(x+y)'''

# approach7
s=input()
x=s[::2]
y=s[1::2]
print(x+y)

# approach5 reverse
s=input()
x=s[::1]
y=s[1::2]
print(y[::-1]+x)
