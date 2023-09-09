# Prime-Number-using-Recursion-in-Python

Prime Number using Recursion
On this page we will learn to create Python Program to Finding out whether  a number is Prime or not using Recursion.

Prime Number : is a number who is completely divisible by 1 and itself only. 

Example :

Input :  971
Output :  Yes, 971 is Prime
Explanation :  971 is Prime as it is completely divisible only by 1 or 971 [itself]
Prime Number in Python
Method 1: Using Recursion
Algorithm
Start by passing value of n to a Function
As we don’t pass any value of i to function by default it gets value 2
If n is equals to i the return True
Else if n is completely divisible by i then return False
Using return keyword call the same function recursively for n, i+1
If returned True print “Yes it is Prime”
Else Print “No it is not Prime”
Python Program to Find Prime number
Python Code
Run
def Prime_Number(n, i=2):
    if n == i:
        return True
    elif n % i == 0:
        return False
    return Prime_Number(n, i + 1)


n = 971
if Prime_Number(n):
    print("Yes,", n, "is Prime")
else:
    print("No,", n, "is not a Prime")
Output :

Yes, 971 is a Prime

Related Pages
Finding Number of times x digit occurs in a given input
 
Finding number of integers which has exactly x divisors
 
Smallest element in an array

Power of a Number

Largest element in an array

Method 2: Using Loop
Algorithm
Start by Passing value of n
Iterate from 2 to half of n
For each iteration check if i completely divides n then return False
After completion of loop return True
If True is returned Print “Yes the Number is Prime”
Else Print “No the Number is not Prime”
Python Code
Run
def Prime_Number(n):
    for i in range(2,1+n//2):
        if n % i == 0:
            return False
    return True


n = 979
if Prime_Number(n):
    print("Yes,", n, "is Prime")
else:
    print("No,", n, "is not a Prime")
Output :

No, 979 is not a Prime
