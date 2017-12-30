# PyPratice1
# 1.1
str1 = input("输入一个人名：")
str2 = input("输入一个国家名：")
print("世界那么大{}想去{}看看。".format(str1,str2))

# 1.2
n = input("请输入一个数：")
sum = 0
for i in range(int(n)):
    sum += i+1
print("和为：",sum)

# 1.3
for i in range(1,10):
    for j in range(1,i+1):
        print("{}*{} = {} ".format(j,i,i*j),end='')
    print(" ")
    
# 1.4
temp,sum = 1,0
for i in range(1,11):
    temp *= i
    sum += temp
print("一到十的阶乘为：{}".format(sum))

# 1.5
n = 1
for i in range(5):
    n = (n+1)*2
print(n)
print("\n")

m = 1
for i in range(5,0,-1):
    m = (m+1)<<1
print(n)

# 1.6
diet = ['牛扒','虾仁','肉丸','米饭','github']
for x in range(0,5):
    for y in range(0,5):
        if not(x == y):
            print("{}配{}，是最棒的了".format(diet[x],diet[y]))
            
# 1.7
from turtle import *
fillcolor("red")
begin_fill()
while True:
    forward(200)
    right(144)
    if abs(pos())<1:
        break
end_fill()

# 1.8
from turtle import *
color('red','yellow')
begin_fill()
while True:
    forward(200)
    left(170)
    if abs(pos())<1:
        break
end_fill()
done()

# 1.9
import turtle
import time
turtle.speed("fastest")
turtle.pensize(2)
for x in range(100):
    turtle.forward(2*x)
    turtle.left(90)
time.sleep(3)

# 1.10
import turtle
import time
turtle.pensize(2)
turtle.bgcolor("black")
colors = ["red","yellow","purple","blue"]
turtle.tracer(False)
for x in range(400):
    turtle.forward(2*x)
    turtle.color(colors[x%4])
    turtle.left(91)
turtle.tracer(True)
