# Ass-2-17-02-2022
Program to print sum of n fibonacci numbers
def calculateSum(n) :

    if (n <= 0) :

        return 0

  
    fibo =[0] * (n+1)

    fibo[1] = 1

  
    # Initialize result

    sm = fibo[0] + fibo[1]

  
    # Add remaining terms

    for i in range(2,n+1) :

        fibo[i] = fibo[i-1] + fibo[i-2]

        sm = sm + fibo[i]

         
    return sm
 
 
# Driver program to test
# above function
n = 4

print("Sum of Fibonacci numbers is : " ,

      calculateSum(n))

Output:
Sum of Fibonacci numbers is : 7
