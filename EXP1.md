# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE: 03/09/24                                                                            
### REGISTER NUMBER : 212221040167

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program.
### Program:
```
a)do...while
def display():
    start=input("Enter a positive value to START")
    end=input("Enter a positive value to END")
    if start.isnumeric()and end.isnumeric():
        while True:
            start=int(start)
            end=int(end)
            print(start,end=' ')
            if start<end:
                start+=1
            else:
                break
    else:
        print("Enter a valid positive value")
        display()

b)while...do
start=input("Enter a positive value for START:")
end=input("Enter a positive value for END:")
if start.isnumeric() and end.isnumeric():
    start=int(start)
    end=int(end)
    while start<=end:
        print(start, end=" ")
        start+=1
else:
    print("Enter a valid positive number")

c)if...else
def switch():
    switcher = {0: "even", 1: "odd"}
    n = input('Enter a value for N: ')
    try:
        n = int(n)
        print(switcher[n % 2])
    except ValueError:
        print("Enter a valid number.")

switch()

d)switch
def compare():
    a=input("Enter a value for A:")
    b=input("Enter a value for B:")
    try:
        a=int(a)
        b=int(b)
        if a>b:
            print("A is greater than")
        elif a<b:
            print("B is greater than")
        else:
            print("A is equal to B")
    except ValueError:
      print("Enter a valid number")
compare()

e)for
def iterate(): 
    string=input("Enter a string: ")
    for i in string: 
        print(ord(i),end=" ")
    print()
     
iterate()
```













### Output:
![Screenshot (158)](https://github.com/user-attachments/assets/cbfb7c05-eb24-44cb-a8e6-c3f016df4c04)
![Screenshot (160)](https://github.com/user-attachments/assets/84b9063f-dc45-4d82-a123-97df9b38471f)
![Screenshot (161)](https://github.com/user-attachments/assets/eabb88c7-f7eb-4d0b-b0cd-b35086f83692)
![Screenshot (163)](https://github.com/user-attachments/assets/c930f166-2a07-4517-94ac-df3892a5400b)







### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


