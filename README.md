# Prime-number-from-list-python-
To find prime numbers from a given set of list and return the output with list of prime numbers, sum and count of prime numbers.

## Python code;
    list_of_numbers = list(map(int, input("Enter all numbers:").split()))

    prime_list = []
    for i in list_of_numbers:
        if i == 0 or i==1:
            pass
        else:
            prime = True
            for j in range(2,int(i/2)+1):
                if i%j == 0:
                    prime = False
                    break
            if prime == False:
                pass
            else:
                prime_list.append(i)

    print(len(prime_list)) #number of prime numbers in a list
    print(sum(prime_list)) #sum of all prime numbers
    print(prime_list) #list of prime numbers
