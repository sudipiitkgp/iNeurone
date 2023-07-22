```python
for i in range(12):
    print(i)
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    11
    


```python
for i in range(0,12,3): 
    print(i)
```

    0
    3
    6
    9
    


```python
l = [1,2,3,"paik","df",556055]
for i in l :
    pass #pass fn blank output
```


```python
#for loop must have proper indentation
for i in "Sudip Paik" :
    print(i)
```

    S
    u
    d
    i
    p
     
    P
    a
    i
    k
    


```python
l = [1,2,3,"paik","df",556055]
for i in l :
    print (i)
else :
    print("Prev Loop Exhausted") #once for loop is completed
```

    1
    2
    3
    paik
    df
    556055
    Prev Loop Exhausted
    


```python
for i in l :
    if i == 3 :
        break # 
    print(i)
else :
    print("this will executed only when for loop is going to complete")
```

    1
    2
    


```python
S = "Sudip_Paik"
for i in S :
    if i == "l" :
        break
    print(i)
else :
    print("Print str", S )
```

    S
    u
    d
    i
    p
    _
    P
    a
    i
    k
    Print str Sudip_Paik
    


```python
t = (4,5,6,7,8,"Sudip")
for i in t:
    print(i)
```

    4
    5
    6
    7
    8
    Sudip
    


```python
s = {2,3,4,5,6,7,7,7,7,7,8,8,8,9}
for i in s :
    print(i)
```

    2
    3
    4
    5
    6
    7
    8
    9
    


```python
s = {2,3,4,5,6,7,7,7,7,7,8,8,8,9}
for i in s :
    print(i)
```


```python
d = {"key1" : "dfwsf" , "key2" : "fsgv" , "key3" : "fscff00"}
for i in d :
    print(i,d[i])
```

    key1 dfwsf
    key2 fsgv
    key3 fscff00
    


```python
d = "* * *"
for i in range(3): #here range signifies no of rows
    print(d)
```

    * * *
    * * *
    * * *
    


```python
for i in range(0, 4): #Outer loop to iterate through each row
    for j in range(0,i+1): #Inner loop to print stars in each row
        print("*", end = " ") #
    print("\n")
```

    * 
    
    * * 
    
    * * * 
    
    * * * * 
    
    


```python
list(range(9,0,-2))
```




    [9, 7, 5, 3, 1]




```python
n = 5
for i in range(5): #iterated from 0-4
    for j in range(0,i+1): 
        print("Sud" , end = " ")
    print("\n")
```

    Sud 
    
    Sud Sud 
    
    Sud Sud Sud 
    
    Sud Sud Sud Sud 
    
    Sud Sud Sud Sud Sud 
    
    


```python
#n = 5: The variable n is assigned the value 5. However, n is not used in the subsequent code.

#Outer loop: for i in range(5):: This loop iterates from 0 to 4 (inclusive) because range(5) generates a sequence from 0 to 4.

#Inner loop: for j in range(0, i+1):: This loop iterates from 0 to the current value of i (inclusive). In the first iteration of the outer loop (i = 0), the inner loop will run once with j taking the value 0.

#print("Sudip", end=" "): This statement prints the word "Sudip" followed by a space without moving to the next line due to the end=" " parameter.

#print("\n"): This statement prints a new line, moving the cursor to the beginning of the next line after the inner loop has finished executing
```


```python
n = 3  # You can change 'n' to any desired number of rows for the triangle

for i in range(n):
    for j in range (i,n-1):
        print(" " * len("Sudip"), end = " ")
    for j in range(i+1):
        print("Sudip" , end = " ")          
    for j in range (i):
        print("Sudip", end=" ")
    print() #new line

```

                Sudip 
          Sudip Sudip Sudip 
    Sudip Sudip Sudip Sudip Sudip 
    


```python
list(range(7))
```




    [0, 1, 2, 3, 4, 5, 6]




```python
t = tuple(range(7))
list(range(len(t)))
```




    [0, 1, 2, 3, 4, 5, 6]




```python
for i in t:
    print(i)
```

    0
    1
    2
    3
    4
    5
    6
    


```python
for i in range(len(t)):
    print(i,t[i]) #index along with respective elements
```

    0 0
    1 1
    2 2
    3 3
    4 4
    5 5
    6 6
    


```python
s = 'ineuron'
for i in range(len(s)):
    print(i,s[i])
```

    0 i
    1 n
    2 e
    3 u
    4 r
    5 o
    6 n
    


```python
s = 'ineuron'
for i in reversed(range(len(s))) :
    print(i,s[i])
```

    6 n
    5 o
    4 r
    3 u
    2 e
    1 n
    0 i
    


```python
d = {"key1" : "dfwsf" , "key2" : "fsgv" , "key3" : "fscff00"}
```


```python
for i in d.items() : #i is tuple and values are at first index 
    print((i), type(i), type(i[1])) #dict to tuples
```

    ('key1', 'dfwsf') <class 'tuple'> <class 'str'>
    ('key2', 'fsgv') <class 'tuple'> <class 'str'>
    ('key3', 'fscff00') <class 'tuple'> <class 'str'>
    


```python

```


```python
#extracting only numbers from list
l = ["sudh","kumar",3234545,"sudh@ineuron.ai",345,3454543]
l1 = []
for i in l:
    if type(i) == int :
        l1.append(i)
print(l1)
```

    [3234545, 345, 3454543]
    


```python
#extract numeric keys with values from dict
d = {1 : 68656 , "name" : "sudp" , 234 : "sdfsfv" , "43" : "sdfefc" , 234 : "3465" }
for i in d:
    if type(i) == int:
        print(i, ":" , d[i])
```

    1 : 68656
    234 : 3465
    


```python
s = "aaaabbccd"
set(s) #conversion to set to get unique elements
```




    {'a', 'b', 'c', 'd'}




```python
s.count('a')
```




    4




```python
for i in set(s) :
    print(i, ":", s.count(i))
```

    a : 4
    c : 2
    b : 2
    d : 1
    


```python
i = 344559202995152522255584444
s = set(str(i))
for j in s:
        print(int(j) , type(int(j)))
```

    2 <class 'int'>
    8 <class 'int'>
    5 <class 'int'>
    3 <class 'int'>
    4 <class 'int'>
    9 <class 'int'>
    0 <class 'int'>
    1 <class 'int'>
    


```python
str(i)
```




    '344559202995152522255584444'




```python

        
```

    3
    3
    


```python
t = ("sudh" , "kumar" , [1,2,3,4,5] ,(3,4,5,6) , {3 : 3 , "key2" : "kumar"})
for i in t:
    if type(i) == list or type(i) == tuple :
        for j in i :
            if j == 3 :
                print(j)
    if type(i) == dict :
        for k,v in i.items() :
            if k == 3 or v == 3 :
                print(k)
                print(v)
```

    3
    3
    3
    3
    


```python
#q1
a = "ineuron"
n = 4
for i in range(4):
    for j in range(0,i+1):
        print(a , end = " ")
    print()
```

    ineuron 
    ineuron ineuron 
    ineuron ineuron ineuron 
    ineuron ineuron ineuron ineuron 
    


```python
p = "aabbbuidfiriiifssss"
d ={}
for i in set(p):
    d[i] = p.count(i)
```


```python
d
```




    {'s': 4, 'r': 1, 'u': 1, 'd': 1, 'b': 3, 'i': 5, 'a': 2, 'f': 2}




```python

```


```python

```


```python

```


```python
#q2
n = 5
for i in range(n):
    for j in range (i,n-1):
        print(" " * len("Sudip"), end = " ")
    for j in range(i+1):
        print("Sudip" , end = " ")          
    for j in range (i):
        print("Sudip", end=" ")
    for j in range ()
    print()
```
