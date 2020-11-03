# findprimarynumberslist
In this program if you will input a number (i)it will give you list of all prime numbers between 2 to i.
# program to check if the number is prime or not

def primeF(i):
    n =2
    if i==2 :
        str = f"{i} is a prime number"
        primeset.append(i)

    elif i==1:
        str = f"{i} is a not prime number"
    else:
        while  n<i:
            if i%n == 0:
                str = f"{i} not a prime number"
                break
            else:
                str = f"{i} a prime number"

            n=n+1


    if str == f"{i} a prime number":
        primeset.append(i)


num = int(input("Enter the 3 digit number"))
primeset = []

if num == 1:
    print("1 is not a prime numner")
else:
    for i in range(1,num+1):
        primeF(i)
    print(f"The prime number in this range will be {primeset}")
