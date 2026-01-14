Python Basics - Strings & Conditional Statements



```python
str1 = "This is a string"  #double quote
```


```python
str2 = 'ApnaCollege' #single quote
```


```python
str3 = """this is a string""" #triple quote
```


```python
str4 = "This is my car's key" #possessive statement with apostopie under dobule quote
```


```python
str5 = "This is a string. We are creating it in python." #two statements can write in different ways
```


```python
str5a = "This is a string." 
str5b = "We are creating it in python."
```

Escape Sequence Characters  - they are use for formatting statements



```python
str6 = "This is a string.\nWe are creating it in python." #used \n for write statement in next line.
print(str6)
```

    This is a string.
    We are creating it in python.
    

Concatenation #use it to combine more than words, characters, statements



```python
str7 = "Apna"
str8 = "College"
final_str = str7 + str8
print (str7 + str8)
print (final_str)
```

    ApnaCollege
    ApnaCollege
    

Measure Lenght 



```python
str7 = "Apna"
str8 = "College"
len1 = len(str7 +str8)
len2 = len(str7 + " " +str8)
print (len1)
print (len2)
```

    11
    12
    

Indexing = start counting from 0



```python
str = "Apna College"
ch = str[5]
print(ch)
```

    C
    


```python
a = "Ravindra Shelke"
b = a[9]
print(b)
```

    S
    

Slicing = Accessing parts of the string



```python
str = "Apna College"
print(str[1:4])
print(str[0:7])
print(str[5:12])
print(str[0:])
```

    pna
    Apna Co
    College
    Apna College
    

Slincing = negative index



```python
str = "Apple"
print(str[-3:-1])
```

    pl
    
#String Functions
#str = "I am a coder."
#str.endswith("er.") #returns true if string ends with substr
#str.capitalize() #capitalizes 1st char
#str.replace(old,new) #replace all occurrences of old with new
#str.find(word) #returns 1st index of 1st occurrence
#str.count("am") #counts the occurrence of substr in string


```python
str1 = "i am a python programer python"
print(str1.endswith("ravi"))
print(str1.capitalize())
print(str1.replace("am","was"))
print(str1.find("python"))
print(str1.count("python"))
```

    False
    I am a python programer python
    i was a python progrwaser python
    7
    2
    


```python
((a+b)(b+c)(c+d)) #tuple
("I am a student") #string
```


```python
str = "I am studying python from ApnaCollege"
print(str.endswith("ege"))
print(str.endswith("rom"))
```

    True
    False
    


```python
str = "i am studying python from ApnaCollege"
print(str.capitalize())
print(str)
str=str.capitalize()
print(str)
```

    I am studying python from apnacollege
    i am studying python from ApnaCollege
    I am studying python from apnacollege
    


```python
str = "I am studying python from ApnaCollege"
print(str.replace("o", "a"))
```

    I am studying pythan fram ApnaCallege
    


```python
str = "I am studying python from ApnaCollege"
print(str.replace("python", "JavaScript"))
```

    I am studying JavaScript from ApnaCollege
    


```python
str = "I am studying python from ApnaCollege"
print(str.find("from"))
```

    21
    


```python
str = "I am studying python from ApnaCollege"
print(str.count("from"))
print(str.count("o"))
```

    1
    3
    

Q. Write a program to input user's first name & print its length


```python
str = "Ravindra Shelke"
print(str(input("first name")))
```

    first name Ravindra
    


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[55], line 2
          1 str = "Ravindra Shelke"
    ----> 2 print(str(input("first name")))
    

    TypeError: 'str' object is not callable



```python
Name = input("enter your name:")
print("length of your name is", len(Name))
```

    enter your name: Ravindra
    

    length of your name is 8
    


```python
rating = input("enter your rating:")
print("lenght of your rating is", len(rating))
```

    enter your rating: Marvallous
    

    lenght of your rating is 10
    

Q. Write a program to find the occurance of '$' in a String


```python
str = "I am $studying python from $ApnaCollege"
print(str.find("$"))
```

    5
    

Q.Write a program to count the occurance of '$' in a String


```python
str = "I $am $studying $python from $ApnaCollege"
print(str.count("$"))
```

    4
    

Conditional Statements
if-elif-else (SYNTAX)


```python
if(condition):
    statement1
elif(condition):
    statement2
else:
    statementN
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[65], line 1
    ----> 1 if(condition):
          2     statement1
          3 elif(condition):
    

    NameError: name 'condition' is not defined



```python
age = 24

if(True):
    print("eligible for vote")
else:
    print("not eligivle for vote")
```

    eligible for vote
    


```python
light = "green"
if(light == "red"):
    print("stop")
elif(light=="green"):
    print("go")
elif(light=="yellow"):
    print("look")
```

    go
    


```python
light = "yellow"
if(light == "red"):
    print("stop")
elif(light=="green"):
    print("go")
elif(light=="yellow"):
    print("look")
```

    look
    


```python
light = "red"
if(light == "red"):
    print("stop")
elif(light=="green"):
    print("go")
elif(light=="yellow"):
    print("look")
```

    stop
    


```python
light = "pink"
if(light == "red"):
    print("stop")
if(light=="green"):
    print("go")
if(light=="yellow"):
    print("look")
else:
    print("light is broken")
```

    light is broken
    

Grade strudents based on marks


```python
marks>=90, grade = "A"
```


```python
90 > marks >=80, grade = "B"
```


```python
80 > marks >=70, grade = "C"
```


```python
70 > marks, grade = "D"
```


```python
marks =74
if(marks >=90):
    grade = "A"
elif(marks >=80 and marks <90):
    grade = "B"
elif(marks >=70 and marks <80):
    grade = "C"
else:
    grade = "D"
print ("Grade of the student ->", grade)
```

    Grade of the student -> C
    


```python
marks =60
if(marks >=90):
    grade = "A"
elif(marks>=80):
    grade = "B"
elif(marks>=70):
    grade = "C"
else:
    grade = "Fail"
print("Grade of the student =>", grade)
```

    Grade of the student => Fail
    


```python
marks =95
if(marks >=90):
    grade = "A"
elif(marks >=80 and marks <90):
    grade = "B"
elif(marks >=70 and marks <80):
    grade = "C"
else:
    grade = "D"
print ("Grade of the student ->", grade)
```

    Grade of the student -> A
    


```python
marks =54
if(marks >=90):
    grade = "A"
elif(marks >=80 and marks <90):
    grade = "B"
elif(marks >=70 and marks <80):
    grade = "C"
else:
    grade = "D"
print ("Grade of the student ->", grade)
```

    Grade of the student -> D
    


```python
marks = int(input("enter student marks:"))
if(marks >=90):
    grade = "A"
elif(marks >=80 and marks <90):
    grade = "B"
elif(marks >=70 and marks <80):
    grade = "C"
else:
    grade = "D"
print ("Grade of the student ->", grade)
```

    enter student marks: 65
    

    Grade of the student -> D
    

#Nesting condition  - means write one statement under another



```python
age = 34
if(age >=18):
    print("can drive")
else:
    print("cannot drive")
```

    can drive
    


```python
age = 95
#nesting
if(age>=18):
    if(age>=80):
        print("cannot drive")
    else:
        print("can drive")
else:
    print("can drive")
```

    cannot drive
    


```python
age = 67
#nesting
if(age>=18):
    if(age>=80):
        print("cannot drive")
    else:
        print("can drive")
else:
    print("can drive")
```

    can drive
    


```python
age = 35
#nesting
if(age>=18):
    if(age>=80):
        print("cannot drive")
    else:
        print("can drive")
else:
    print("can drive")
```

    can drive
    


```python
age = 81
#nesting
if(age>=18):
    if(age>=80):
        print("cannot drive")
    else:
        print("can drive")
else:
    print("cannot drive")
```

    cannot drive
    


```python
age = int(input("age of the person: "))
#nesting
if(age>=18):
    if(age>=80):
        print("cannot drive")
    else:
        print("can drive")
else:
    print("cannot drive")
```

    age of the person:  67
    

    can drive
    

Q. Write a program to check if a number entered by the user is odd or even.


```python
num = 98
remainder = num % 2
if(remainder == 0):
    print("even")
else:
    print("odd")
```

    even
    


```python
num = 66
remainder = num % 2
if(remainder == 0):
    print("even")
else:
    print("odd")
```

    even
    


```python
num = int(input("enter number = "))
remainder = num % 2
if(remainder == 0):
    print("even")
else:
    print("odd")
```

    enter number =  57
    

    odd
    


```python
num = 73

if(num % 2 == 0):
    print("even")
else:
    print("odd")
```

    odd
    


```python
num = int(input("enter number = "))

if(num % 2 == 0):
    print("even")
else:
    print("odd")
```

    enter number =  95
    

    odd
    

Q. Write a program to find the greatest of 3 numbers entered by the user.


```python
a = int(input("enter first number:"))
b = int(input("enter second number:"))
c = int(input("enter third number:"))
if(a >= b and a >= c):
    print("fist number is greatest", a)
elif(b >= a and b >= c):
    print("sencond number is greatest", b)
elif(c >= a and c >= b):
    print("third number is greatest", c)
else:
    print("All are smallest")
```

    enter first number: 35
    enter second number: -87
    enter third number: 56
    

    third number is greatest 56
    

Q. Write a program to check if a number is a multiple of 7 or not


```python
X = int(input("enter number: "))

if(X%7 == 0):
    print("multiple of 7")
else:
    print("not a multiple of 7")
```

    enter number:  45
    

    not a multiple of 7
    


```python
a = int(input("enter number:"))

if (a%8 == 0):
    print("multiple of 8")
else:
    print("not a multiple of 8")
```

    enter number: 78
    

    not a multiple of 8
    


```python
X = int(input("enter number: "))

if(X%7 == 0):
    print("multiple of 7")
else:
    print("not a multiple of 7")
```

    enter number:  49
    

    multiple of 7
    


```python
for i in range(5):
    print("Iteration:", i)
```

    Iteration: 0
    Iteration: 1
    Iteration: 2
    Iteration: 3
    Iteration: 4
    


```python
a = 4
b = 6
c = +(a+b)-4
print(c)
```

    6
    


```python

```
