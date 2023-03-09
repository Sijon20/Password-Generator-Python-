# Password-Generator
This programme is for generate random password through your input length 

Code is -
```
import random
Ual = "QWERTYUIOPASDFGHJKLZXCVBNM"
Lal ="qwertyuiopasdfghjklzxcvbnm"
num ="1234567890"
sym ="!@#$%^&*()_+=-{[}]\|:;.>,</?"
nu = ["1","2","3","4"]
i = 1
password=""

len= int(input("Enter the length of Password: "))
if (len <=100000):
  
  while(i<=len):
    numa=random.choice(nu)
    if (numa=='1'):
        password+= random.choice(Ual)
    elif(numa=='2'):
        password+=random.choice(Lal)
    elif(numa=='3'):
        password+= random.choice(num)
    else:
        password+=random.choice(sym)
    i=i+1

  print("Ypur Password: ",password)
else:
  print("Your Password Length Must Be Under 100,000")
  ```
