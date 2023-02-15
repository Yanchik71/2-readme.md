# 2-readme.md
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
| 7 | |
| 8 | |
| 9 | |
| 10 | |
| 11 | |
| 12 | |
| 13 | |
| 14 | |
| 15 | |
| 16 | |
| 17 | |
| 18 | |
| 19 | |
| 20 | |
| 21 | |
| 22 | |
| 23 | |
| 24 | |
| 25 | |
| 26 | |
| 27 | |
from turtle import *
left(90)
for i in range(7):
    forward(300)
    right(120)
pu()
for x in range(1,9):
    for y in range(1,10):
        goto(x*30,y*30)
        dot(5)
done()

Генерируе все возможные числаь
Рассматриваемкаждое число( сторку) на удовлетвоериение условию задач9 самые ходовые используемые  с cound() 
ели число продит по всем проверкам мы выводим счетчик правильных значений , 

Команды для черепешкаи
  движение вперед Worfard в качестве аргумента пишем число пикселей 
  left, right  повороты влево и вправо
   go to  идти на позицию ( 
   dot толщина точки 
   
   from itertools import product
nums=product('01234',repeat=8)
n='16 36 56 76 61 63 65 67'
nn=n.split()
for x in nums:
    n=''.join(x)
    print(n )
    
    
    
    
    16 задание
 import sys
setrecursionlimit (3050)
def f(n):
    if n<3:
         return 2
    elif n>2 and n&2==0:
         return (f(n-1)+f(n-2)-n)
    elif n>2 and n&2==1:
       return (f(n-2)-f(n-1)+2*n)  
print (f(30))
   
