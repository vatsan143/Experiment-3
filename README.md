# Experiment-3

## PRIME NUMBER OR NOT

## Aim: Write a python program to check the number is prime or not and inspect for failures. 

## Algorithm
1. Start the program.
2. Get the number to be checked from the user.
3. If the number is less than or equal to 1, return "Not Prime".
4. If the number is 2, return "Prime".
5. Start the iteration from 3, For each iteration:
 - If the number is divisible by the current iteration value, return "Not Prime".
6. If the number is not divisible by any value from 2 to the square root, return "Prime".
7. Stop the program. 

## Program
#### NAME: SRIVATSAN
#### REG NO: 212223230216
```
num = input("Enter a number: ")  
flag = 0  

if num.isnumeric():  
    z = int(num)  

    if z == 2:  
        flag = 1  
    elif z > 2:  
        for i in range(2, z // 2 + 1):  # Loop should include z//2
            if z % i == 0:  
                flag = 0  
                break  
        else:  
            flag = 1  

    if flag == 1:  
        print("Prime Number")  
    else:  
        print("Not a Prime Number")  

else:  
    print("Enter a Positive Number")

```
## Output
<img width="692" height="174" alt="image" src="https://github.com/user-attachments/assets/bde20c37-28fc-4161-9aaf-54c945e4168e" />

## Result
Thus, the python program to check the number is prime or not and inspect for failures is executed successfully.
