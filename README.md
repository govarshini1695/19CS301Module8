# 19CS301Module8
EXPTNO.8a Program to find Find the simple interest

### Aim: To Write a Python Program to find Find the simple interest by getting the principal, rate and time value from the user.

### Algorithm:

STEP 1: Start.
STEP 2: Define a function.
STEP 3: Create variable 'p','r','t' for principal,rate of interest and time.
STEP 4: Get the input of p,r and t from user.
STEP 5 : Using the formula (p*r*t)/100 calculate the result. 
STEP 6: Print the result.
STEP 7: Stop.

### Program:
```
def simpleInterest(p,t,r):
    si=(p*t*r)/100
    return si
p,r,t=eval(input()),eval(input()),eval(input())

```
### Output:
![image](https://github.com/user-attachments/assets/0cc71222-9697-4545-a937-b330407cbc02)

### Result: Thus, the given program is implemented and executed successfully .

EXPTNo.8b Python program to replace the substring

### Aim: To Write a python program to find the first appearance of the substring 'not' and 'poor' from a given string, if 'not' follows the 'poor', replace the whole 'not'...'poor' substring with 'good'. 

### Algorithm:

STEP 1:Start.
STEP 2:Read a string str1 from the user.
STEP 3:Locate the index of "not" in the string (snot).
STEP 4:Locate the index of "poor" in the string (spoor).
STEP 5:If "poor" appears after "not" and both words exist in the string (snot > 0 and spoor > 0):Replace the substring "not...poor" with "good".
STEP 6 :If the condition is met, return the modified string; otherwise, return the original string.
STEP 7:Stop.

### Program:
```
def not_poor(str1):
    snot=str1.find('not')
    spoor=str1.find('poor')
    if spoor > snot and snot>0 and spoor>0:
        str1=str1.replace(str1[snot:(spoor+1)],'good')
        return str1
    else:
        return str1
print(not_poor('The lyrics is good!'))
```
### Output:
![image](https://github.com/user-attachments/assets/5f7d252f-10af-4394-b4b9-a423f277270d)

### Result: Thus, the given program is implemented and executed successfully .
 

EXPT NO>8C Python Program to print runner up score.

AIM:
To create a python program to find the runner-up score from the  participants' score sheet of n scores for your University Sports Day.  

### Algorithm:
STEP 1:Start.
STEP 2:Read an integer n (size of the array).
STEP 3:Take n space-separated integers as input and store them in a list arr.
STEP 4:Sort arr in ascending order.
STEP 5:Assign large = arr[-1] (last element).
STEP 6:Reverse arr to arrange it in descending order.
STEP 7:Traverse the reversed list to find the first element smaller than the largest.
STEP 8:Stop at the first smaller number and print it.
STEP 9:Terminate the program.

### Program:
```
n = int(input())
arr = list(map(int, input().split()))
arr.sort()
large=arr[-1]
arr.reverse()
for i in range(len(arr)-1):
    if arr[i+1]<arr[i]:
        print(arr[i+1])
        break
```
### Output:

![image](https://github.com/user-attachments/assets/57cbbdea-bc84-4015-823b-ff55726879e0)

### Result: Thus, the given program is implemented and executed successfully .


EX: 8.d  Square all the even numbers and Cube all odd numbers

### Aim: To Develop a python program to square all the even numbers and cube all odd numbers from a list of integers. Get the starting and ending range to create a list.


### Algorithm:

STEP 1:Start.
STEP 2:Create a variable f and l for upper and lower limit of list.
STEP 3:Get the value of f and l from user.
STEP 4:Create a list.
STEP 5:Get the input from user and append in the list.
STEP 6:Create a lambda function to calculate the result.
STEP 7:Print the result.
STEP 8: Stop.

### Program:
```
cube=lambda x:x**2 if x%2==0 else x**3
def fun(f,l):
    l1=[]
    for i in range(f,l+1):
        l1.append(i)
    return l1
f,l=int(input()),int(input())

```
### Output:

![image](https://github.com/user-attachments/assets/6bea817b-4e96-4265-a3c8-3abf23ffa14a)


### Result: Thus, the given program is implemented and executed successfully .
 

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



