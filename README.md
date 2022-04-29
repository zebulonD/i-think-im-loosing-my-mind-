# i-think-im-loosing-my-mind-
this is a visual insight into my magical mind 




import math

num1=list()
sign2=list()
num2=list()
eq=list()
sum1=list()



global x
global y
global sign
global som
som = 0




def add():

    global x
    global y

    x=input("x")
    y=input("y")
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

def sub():

    global x
    global y

    
    x=input("x")
    y=input("y")
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


def muti():

    global x
    global y

    
    x=input("x")
    y=input("y")
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


def divide():

    global x
    global y

    
    x=input("x")
    y=input("y")
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


def history():
    print(num1)
    print(sign2)
    print(num2)
    print(eq)
    print(sum1)





while True:
    

    while True:
        print("ans")
        ans=input()

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
        elif ans=="end":
            quit()
        else:
            print("try again")




    

    history = [[0,0,0,0,0,0,0,0,0,0,0,0,0,0],[0]]
    history.append(0,0(2))
   
    print (history)


    x= str(x)
    y=str(y)
    som = str(som)

    num1.append(x)
    sign2.append(sign)
    num2.append(y)
    eq.append('= ')
    sum1.append(som)

