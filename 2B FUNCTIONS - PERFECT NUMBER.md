# Exp.No:2b  
## FUNCTIONS - STRONG NUMBER

### AIM  
To create a Python program using a function to check whether a given number is a strong number or not.

---

### ALGORITHM

1.	Begin the program.
2.	Define a function strong(num) to check if the given number is a strong number.
3.	Inside the function, initialize sum = 0 and store the original number in a temporary variable t.
4.	Use a while loop to extract each digit of the number:
5.	Set i = 1 and f = 1 for factorial calculation.
6.	Find the last digit r using r = t % 10.
7.	Calculate the factorial of r using another while loop.
8.	Add the factorial to sum.
9.	Remove the last digit by updating t = t // 10.
10.	After the loop ends, compare sum with the original number:
11.	If they are equal, print "The number is a strong number".
12.	Else, print "The number is not a strong number".
13.	Read an integer input from the user.
14.	Call the strong() function with the input number.
15.	Terminate the program.

---

### PROGRAM
```
#Reg.No:212223060200
#Name:Pradeep M
#Add your Code Here

def strong(num):
    sum=0
    t=num
    while(t>0):
        i=1
        f=1
        r=t%10
        while(i<=r):
            f*=i
            i+=1
        sum+=f
        t//=10
    
    if(sum==num):
        print("The number is a strong number")
    else:
        print("The number is not a strong number")
        
a=int(input())
strong(a)
```
### OUTPUT

<img width="1155" height="272" alt="437954486-59da4f37-b861-4946-98ab-bbc55573ee1e" src="https://github.com/user-attachments/assets/c80a191a-9eb1-4bea-983f-1707c258760e" />



### RESULT
Thus, the Python program to check whether a given number is a strong number or not using a function has been implemented and executed successfully.
