# 2-readme.md

    ## Задачи ЕГЭ
| задание из ЕГЭ |выполнено |
| ------ | ------ |
| 1 | |
| 2 | + |
| 3 | |
| 4 | |
| 5 | + | 
| 6 | + |
| 7 | |
| 8 | + |
| 9 | |
| 10 | |
| 11 | |
| 12 | + |
| 13 | |
| 14 | + |
| 15 | + |
| 16 | + |
| 17 | + |
| 18 | |
| 19 | + |
| 20 | + |
| 21 | + |
| 22 | + |
| 23 | + |
| 24 | + |
| 25 | + |
| 26 | + |
| 27 | |


#Уникальные команды#

1. print('a')
2. def f(c):
3. for i in range():
4. readline
5. elif c<a:
6. else: 
7. while
8.return 
9. int
10. input
11. from turtle input
12. with open
13. left
14.  forward
15.  right
16.   goto
17.  dot
18.   done
19.   break
20. nums=product  
21. split()
22. import  


#5
  ```python
  for N in range (516):
    b = f'{N:b}'
    if N % 2 == 0:
        b += '10'
    else:
        b = '1'+ b + '01'
    if int(b,2)>516:
         print(N)
         break
   ```
    
#6
  ```python
  from turtle import *
  left(90)
  for i in range (7):
    forward(300)
    right(120)
  pu()
  for x in range (1,9):
    for y in range (1,10):
      goto(x*30, y*30)
      dot(5)
   done()
   ```
   
   ```python
   from turtle import *
left(90)
for i in range (1):
  forward(150)
  right(90)
  forward(150)
  goto(0, 0)
pu()
for x in range (0,15):
  for y in range (0,15):
    goto(x*10, y*10)
    dot(2)
done()
```
   
   
   
   


#8

```python 
from itertools import product
nums=product('01234567',repeat=6)
k=0
n='16 36 56 76 61 63 65 67'
nn=n.split()
for n in nums:
    numb=''.join(n)
    sp=[]
    if numb.count('6')==1 and numb[0]!='0':
        for x in nn:
            if x in numb:
                sp.append(x)
        if not sp: 
            k+=1
print(k)

```



#12


```python
spisok=[]
for num in range(2,1000):
    if all(num%delit!=0 for delit in range (2, num-1)):
        spisok.append(num)
flag=False
for i in spisok:
    for y in range (100):
        if y*4+117==i and flag==False:
            print(y, i)
            flag=True
```





#14


```python
a='0123456789abcde'
for x in a:
    f=int(f'123{x}5',15)+int(f'1{x}233',15)
    if  f%14 ==0:
        print(f//14)
        break
 ```
 
 
 #15
 ```python
 
 for A in range(1,1000):
   if all(((x%2==0)<=(x%3!=0)) or (x+A>=100) for x in range (1,100)):
        print(A)
        break
 ```

#16
 
 ```python 
 import sys
sys.setrecursionlimit(3050)
def f(n):
    if n==1: return 1
    elif n>1: return n*f(n-1)
print(f(2023)/f(2020))
```

```python
it1=1
it2=1
for i in range (1, 2024):
    it1=it1*i
for i in range (1, 2021):
    it2=it2*i
print(it1/it2)
```

#17

 ```python
 with open('17.txt') as f:
    nums=[int(x)for x in f]
    c=list(map(abs,nums))
    count=0
    sp=[]
    for i in range(len(nums)-1):
        if abs(nums[i])%10==3:
            sp.append(nums[i])
    maxi=max(sp)**2
    sqrt=[]
    for i in range(len(c)-1):
        if ((c[i]%10==3 and c[i+1]%10!=3 ) or (c[i]%10!=3 and c[i+1]%10==3)) and (c[i]**2+c[i+1]**2)>=maxi:
            count+=1
            sqrt.append(c[i]**2+c[i+1]**2)
    print(count)
    print(max(sqrt))
 ```


#23

 ```python
from itertools import product
def f (x, y, z):
    count=0
    for i in range(2,z):
        print(i)
        b=product('12',repeat=i) 
        for n in b: 
            a=x
            if x==10 and n.count('2')>1:continue 
            for l in n: 
                if l=='1': a+=1 
                else: a*=2
                if a==17:break
            if a==y: count+=1
    return count
g=f(10, 35, 24)
r=f(1,10, 10)
print(g*r)
```

#24
```python
with open('24.txt') as f:
    s=f.readline().replace('C','S').replace('D','S').replace('F','S')
    s=s.replace('A','G').replace('O','G')
    s=s.replace('SG','*')
    k=kmax=0
    for i in s:
        if i=='*':
            k+=1
            kmax=max(k,kmax)
        else:k=0
print(kmax)

```


#25
```python
for i in range (2023,10**10,2023):
    n=str(i)
    if n[0]=='1' and n[2:6]=='2139' and n[-1]=='4': print(i,i/2023)

```

    
#26
```python
with open('26.txt') as f:
    s=[int(x) for x in f]
    s.pop(0)
    s.sort(reverse=True)
    k,mini=1,s[0]
    for i in range(1, len(s)):
        if s[i]+3<=mini:
            mini=s[i]
            k+=1
    print(k, mini)

```
#25
```python
for i in range (17,10**11,17):
    n=str(i)
    if n[0:5]=='12345' and n[5]=='6' and n[-1]=='8': print(i,i/17)
    
    ```
    ```
    #Справочник команд#

``` 
 ( ¬) - not - Логическое отрицание, инверсия — логическая операция, в результате которой из данного высказывания (например, А) получается новое высказывание (не А)
 ``` 
 ``` 
 ( ∨ )- or-  Дизъюнкция  — логическое сложение, операция, соединяющая два или более высказываний при помощи связки «или» (например, «А или В»)
 
 ```
 ``` 
( ∧ )- and- Конъюнкция — логическое умножение, операция, требующая как минимум двух логических величин (операндов) и соединяющая два или более высказываний при помощи связки «и» (например, «А и В»)
 ```
 ``` 
  ( ≡ ) - == -Эквивалентность, двойная импликация, равнозначность — логическая операция, позволяющая из двух высказываний А и В получить новое высказывание А ≡ В
  ``` 
 ```
( → ) Импликация — логическая операция, соединяющая два высказывания при помощи связки «если..., то» в сложное высказывание, которое символически обозначается с помощью знака → (А → В) 
 ```
 
 1. print  — функция вывода (например в консоль);  
 print('x y z w')
 print(f')
  ``` 
2. range — вернет последовательность чисел, с 0 до N (с шагом на 1 по умолчанию);
``` 
3. dir — список имен объекта (если он указан) или список объектов доступных в локальной области (если объект не указан);
``` 
4. divmod — вернет частное и остаток от деления двух чисел;
``` 
 5. numerate  — вернет объект, который генерирует кортежи из двух элементов (индекса и самого элемента);
 ``` 
6. format — форматирование (например форматирование строки);
``` 
7. globals — глобальные имена (в виде словаря);
``` 
8. locals — локальные имена (в виде словаря);
``` 
9. help — вызовет встроенную справку;
``` 
10. input — вернет введенную пользователем строку;
``` 
11. open — откроет файл и вернет его объект.Справочник команд python 
``` 
12. abs — возвращает модуль числа; 
```
