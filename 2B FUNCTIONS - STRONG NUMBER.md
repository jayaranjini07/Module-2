# Exp.No:2b  
## FUNCTIONS - STRONG NUMBER

### AIM  
To write a python program to check if a number is a strong number using function.

---

### ALGORITHM
1.Start

2.Input a number n

3.Store the original number in a temporary variable temp = n

4.Initialize sum1 = 0 to store the sum of factorials of digits

5.Repeat the following steps while n > 0:

a. Get the last digit: r = n % 10

b. Initialize f = 1 (to calculate factorial)

c. Calculate the factorial of r:

For i = 1 to r, multiply f = f * i

d. Add factorial to sum: sum1 = sum1 + f

e. Remove the last digit: n = n // 10

6.Compare sum1 with temp:

If sum1 == temp, then print: "The number is a strong number"

Else, print: "The number is not a strong number"

7.End

---

### PROGRAM
```
#Reg.No:212223060101
#Name:JAYA RANJINI S

def strong(num):
    sum1=0
    temp=num
    while(num):
        i=1
        f=1
        r=num%10
        while(i<=r):
            f=f*i
            i=i+1
        sum1=sum1+f
        num=num//10
    if(sum1==temp):
        print("The number is a strong number")
    else:
         print("The number is not a strong number")
    
    
n=int(input())
strong(n)
```
### OUTPUT

![image](https://github.com/user-attachments/assets/64624e4e-4df4-4f75-9048-1288483a26ab)

### RESULT
Thus the python program to check if a number is a strong number using function was implemented and executed successfully.
