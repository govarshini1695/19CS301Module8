HACKERRACK CHALLENGES

AIM: 
To write a python program to perform the given commands like insert,print,delete,insert at end,sort,
pop,reverse the list.

ALGORITHM:
STEP 1:Start
STEP 2:Initialize an empty list l.
STEP 3:Take input N, which defines the number of commands to be executed.
STEP 4:Loop through N times:
   Read a command string and split it into a list s.
   Check the first element (s[0]) to determine the operation:
        "insert" → Insert s[2] at position s[1] in l.
        "remove" → Remove the element s[1] from l.
        "append" → Add s[1] to the end of l.
        "pop" → Remove the last element of l.
        "sort" → Sort the list l in ascending order.
        "reverse" → Reverse the order of elements in l.
        "print" → Print the current state of l.
STEP 5:End the loop after processing all N commands.
STEP 6:End

PROGRAM:
```
N=int(input())
l=[]
for i in range(N):
    s=input().split()
    if s[0]=='insert':
        l.insert(int(s[1]),int(s[2]))
    elif s[0]=='remove':
        l.remove(int(s[1]))
    elif s[0]=='append':
        l.append(int(s[1]))
    elif s[0]=='pop':
        l.pop()
    elif s[0]=='sort':
        l.sort()
    elif s[0]=='reverse':
        l.reverse()
    elif s[0]=='print':
        print(l)
```

OUTPUT:
![image](https://github.com/user-attachments/assets/02d6a119-2db2-496c-a47d-5d36163ac7bd)



RESULT:
Thus the python program to perform the given commands like insert,print,delete,insert at end,sort,
pop,reverse the list is executed successfully.


