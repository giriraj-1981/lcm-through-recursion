# lcm-through-recursion
# This function computes GCD 
def compute_gcd(x, y):
    while y%x!=0:
        r=y%x
        y=x
        x=r

    return x

   

# This function computes LCM
def compute_lcm(x, y):
   lcm = (x*y)//compute_gcd(x,y)
   return lcm

#num1 = 54
#num2 = 24
num1=int(input("input first number to find lcm"))
num2=int(input("input second number to find lcm"))

print("The L.C.M. is", compute_lcm(num1, num2))
