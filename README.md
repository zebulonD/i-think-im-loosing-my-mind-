# i-think-im-loosing-my-mind-
this is a visual insight into my magical mind 








import math
import time



t=("welcome","to the","grand","Zebbby D","calculator ","","")
for f in t:
    print(f)
    time.sleep(0.5)

alpha=("please type \"+\" if you wish to add",
       "please type \"-\" if you wish to take away",
       "please type \"*\" if you wish to multiply",
       "please type \"/\" if you wish to devide",
       "please type \"end\" if you wish to end this program",
       "please type \"history\" if you wish to see your previous calculations",
       "please type \"previous\" if you wish to use a previous answer in your next calculation \nhowever it is unavailble untill your first caculation",
       "please type \"menu\" if you wish to see what options you have","","")
for you in alpha:
    print(you)
    time.sleep(0.5)




global x

global y
global sign
global som
som = 0
H = [[],[],[],[],[],[]]

global prv
prv=0


def add():
    global j
    j=1

    global x
  
    global y
    global prv
    global pos
    
    if prv ==1:
        x=H[5][pos]
        print(x)
    else:
        x=input()
    prv=0

        
    
    print("+")
    y=input()
    if x == "pi":
        x=math.pi
    else:
        x=int(x)    
    if y == "pi":
        y=math.pi
    else:
        y=int(y)

    global sign
    global som
    sign = "+"
    som = x+y

    print("---------------------------------------------------------------------------------------------------------------------")
    print(x)
    print(sign)
    print(y)
    print("=")
    print(som)
    print("---------------------------------------------------------------------------------------------------------------------")

    x= str(x)
    y=str(y)
    som = str(som)
    

    H[0].append("")
    H[1].append(x)
    H[2].append(sign)
    H[3].append(y)
    H[4].append("=")
    H[5].append(som)

 

    

def sub():
    global j
    j=1

    global x
   
    global y
    global prv
    global pos

    if prv ==1:
        x=H[5][pos]
        print(x)
    else:
        x=input()
    prv=0


    print("-")
    y=input()
    if x == "pi":
        x=math.pi
    else:
        x=int(x)    
    if y == "pi":
        y=math.pi
    else:
        y=int(y)

    global sign
    global som
    sign = "-"
    som = x-y

    print("---------------------------------------------------------------------------------------------------------------------")
    print(x)
    print(sign)
    print(y)
    print("=")
    print(som)
    print("---------------------------------------------------------------------------------------------------------------------")

    x= str(x)
    y=str(y)
    som = str(som)

    H[0].append("")
    H[1].append(x)
    H[2].append(sign)
    H[3].append(y)
    H[4].append("=")
    H[5].append(som)

   


def muti():
    global j
    j=1

    global x
  
    global y
    global prv
    global pos

    
    
    if prv ==1:
        x=H[5][pos]
        print(x)
    else:
        x=input()
    prv=0


    print("-")
    y=input()
    if x == "pi":
        x=math.pi
    else:
        x=int(x)    
    if y == "pi":
        y=math.pi
    else:
        y=int(y)

    global sign
    global som
    sign = "*"
    som = x*y

    print("---------------------------------------------------------------------------------------------------------------------")
    print(x)
    print(sign)
    print(y)
    print("=")
    print(som)
    print("---------------------------------------------------------------------------------------------------------------------")

    x= str(x)
    y=str(y)
    som = str(som)

    H[0].append("")
    H[1].append(x)
    H[2].append(sign)
    H[3].append(y)
    H[4].append("=")
    H[5].append(som)

   


def divide():
    global j
    j=1

    global x
    
    global y
    global prv
    global pos

    
    
    if prv ==1:
        x=H[5][pos]
        print(x)
    else:
        x=input()
    prv=0


    print("-")
    y=input()
    if x == "pi":
        x=math.pi
    else:
        x=int(x)    
    if y == "pi":
        y=math.pi
    else:
        y=int(y)

    global sign
    global som
    sign = "/"
    som = x/y

    print("---------------------------------------------------------------------------------------------------------------------")
    print(x)
    print(sign)
    print(y)
    print("=")
    print(som)
    print("---------------------------------------------------------------------------------------------------------------------")

    x= str(x)
    y=str(y)
    som = str(som)

    H[0].append("")
    H[1].append(x)
    H[2].append(sign)
    H[3].append(y)
    H[4].append("=")
    H[5].append(som)
   

    


def history():
    global t
    g=0
    print("---------------------------------------------------------------------------------------------------------------------")
    for p in H[0]:
        
        i = g +1
        print("calculation",i)
        print("")
        print(H[1][g])
        print(H[2][g])
        print(H[3][g])
        print(H[4][g])
        print(H[5][g])
        print("")
        print("")
        g+=1

    print("---------------------------------------------------------------------------------------------------------------------")
  
def previus():
    global prv
    global pos
    g = input("what calculation number was it ? \n or if it was your last calculation please type\"last\" \n ")
    u=int(g)
    while True:
        if u == int(u):
             u=int(u)
             u-=1
             pos= u
             print(H[5][u])
             break
        elif g =="last":
            g =len(H[0])
            pos=g
            print(H[5][g])
            break
        else:
            print("sorry that isnt valid")
        break




   

    

def menu():
    print("please type \"+\" if you wish to add")
    print("please type \"-\" if you wish to take away")
    print("please type \"*\" if you wish to multiply")
    print("please type \"/\" if you wish to devide")
    print("please type \"end\" if you wish to end this program")
    print("please type \"history\" if you wish to see your previous calculations")
    print("please type \"previous\" if you wish to use a previous answer inn your next calculation")
    print("please type \"menu\" if you wish to see what options you have")



global j
j =0

while True:
    

    while True:
        
        print("ans")
        ans=input()
        print("\n")

        if j==1:

            if ans=="add"or ans == "+":
                add()
                break
            elif ans=="sub"or ans == "-":
                sub()
                break
            elif ans=="muti"or ans == "*":
                muti()
                break
            elif ans=="devide"or ans == "/":
                divide()
                break
            elif ans=="history":
                history()
                break
            elif ans=="end"or ans == "exit":
                quit()
            elif ans=="menu":
                menu()
            elif ans =="prv":
                previus()
            else:
                print("try again")

        else:
            if ans=="add"or ans == "+":
                add()
                break
            elif ans=="sub"or ans == "-":
                sub()
                break
            elif ans=="muti"or ans == "*":
                muti()
                break
            elif ans=="devide"or ans == "/":
                divide()
                break
            elif ans=="history":
                history()
                break
            elif ans=="end"or ans == "exit":
                quit()
            elif ans=="menu":
                menu()
            else:
                print("try again")
        
