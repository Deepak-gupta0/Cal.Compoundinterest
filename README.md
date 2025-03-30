# Cal.Compoundinterest
#This python code calculates the compound interest by taking user input of priciple value ,interest and time interval
principle = 0
rate = 0
time = 0

while principle<= 0:
    principle = float(input("enter the principle amount :"))
    if principle <= 0:
        print("principle amount cant be less than or equal to zero ")

while rate<= 0:
    rate = float(input("enter the interest rate :"))
    if rate<= 0:
        print("rate cant be less than or equal to zero ")

while time<= 0:
    time = float(input("enter the time :"))
    if time <= 0:
        print("time cant be less than or equal to zero ") 
        

step1 = (rate/100) + 1 
step2 = step1**time
step3 = step2*principle

print(f"Your compound Interest is : {round(step3,3)}")
         
