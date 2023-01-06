## Assignment Part-1

<b> Q1. Why do we call Python as a general purpose and high-level programming language? in blue </b>

```
Python is called a general-purpose programming language because it can be used to build a wide variety of applications. This means that Python is not designed for a specific task or domain, like some programming languages are. Instead, it is designed to be flexible and versatile, so that it can be used in a wide range of contexts.

Python is also called a high-level programming language because it is relatively abstract and easy to read and write. This means that it is not as close to the underlying machine code of a computer as low-level languages, such as assembly language. Instead, Python provides a higher level of abstraction, which makes it easier for programmers to write and understand code.
```
</br>

<b> Q2. Why is Python called a dynamically typed language? </b>

```
Python is called a dynamically typed language because the type of a variable is determined at runtime, rather than being fixed when the variable is declared. This means that the same variable can be assigned different types of values at different points in the program, depending on the context in which it is used.

It allows the program to handle a wider range of inputs, since variables can be used to hold values of different types.

On the other hand, the disadvantage of dynamic typing is that it can make the program less predictable and more error-prone.

```

</br>

<b> Q3. List some pros and cons of Python programming language? </b>
-> 

</br>

```
Pros :

- Beginner-friendly	
- Large Community	
- Flexible and Extensible	
- portable

Cons : 
- slower then other languages
- It is dynamically typed, which can make the program less predictable and more error-prone.
- multi threading is myth in 
- It does not support static type checking, which means that type errors can only be detected at runtime.
```

</br>

<b> Q4. In what all domains can we use Python? </b>

```
- Web Development : front end and backend
- Data science and machine learning
- IOT 
- Automation
- Game development
- Desktop application
```

</br>
<b> Q5. What are variable and how can we declare them? </b>

</br>

```
-> Python Variable is containers which store values. it can declared by simply assigning a value.
```

</br>

<b> Q6. How can we take an input from the user in Python? </b>

```
-> we can take input through Input() function. it returns the entered text as a string.
```
</br>


<b> Q7. What is the default datatype of the value that has been taken as an input using input() function? </b>
```
-> default datatype is string for input() function
```
</br>


<b> Q8. What is type casting? </b>

```
-> type casting is process of converting  one datatype to the other datatype.
``` 

</br>

<b> Q9. Can we take more than one input from the user using single input() function? If yes, hono, why? </b>w? If 

```
-> yes we can take more than one input from the user by adding split function with input() function. user have to seprate his input though some kind of delimiter such as space.

```

</br>

<b>Q10. What are keywords? </b>
```

->  keywords are reserved words that have special meanings in the language. These words are used to represent specific concepts or language constructs, and they cannot be used as variable names or other identifiers.

There are 33 keywords
```
</br>

<b> Q11. Can we use keywords as a variable? Support your answer with reason. </b>
```
-> keywords can not be used as a variable because keywords are reserved words.
```
</br>


<b> Q12. What is indentation? What's the use of indentaion in Python? </b>

```
-> indentation in python is white space added before code. indentation in python is used to denote block of code.
```

</br>


<b> Q13. How can we throw some output in Python? </b>

```
-> output in python can be given through print() function.
```

</br>

<b> Q14. What are operators in Python? </b>

```
-> Operators are used to perform operations on variables and values.
``` 

</br>

<b> Q15. What is difference between / and // operators? </b>

```
-> both are division operators single slash return answer in float and double slash return answer in integer 
```

</br>

<b> Q16. Write a code that gives following as an output. </b>

```
iNeuroniNeuroniNeuroniNeuron

print("iNeuroniNeuroniNeuroniNeuron")
```

</br>


<b> Q17. Write a code to take a number as an input from the user and check if the number is odd or even. </b>

-> 
```
num = int(input("enter num"))
if num % 2 == 0 :
    print("Number is even")
else:
    print("Number is odd")
```

</br>

<b> Q18. What are boolean operator? </b>

-> Boolean operators are operators that return "true" or "false".
boolean operators :
- Comparison operators
    - ==	
    - !=	
    - <
    - \>
    - <=
    - \>=

- Logical Operators
    - and
    - or 
    - not 

</br>

<b> Q19. What will the output of the following? </b>

ans ->
 
```
1 or 0   --> 1


0 and 0  --> 0

"true" and "false" and "true"  --> "false"

1 or 0 or 0 -- > 1
```

<b> Q20. What are conditional statements in Python? </b>

```
conditional statements are used to execute code only if a certain condition is met. These statements allow the program to make decisions based on the values of variables or expressions, and they are an essential part of many programming tasks.

Python provides several different types of conditional statements, including if, if...else, and if...elif...else statements.
```

</br>



<b> Q21. What is use of 'if', 'elif' and 'else' keywords? </b>

```
-> use of if keyword is to add conditions in the code. elif is used to add alternate conditions. alternate condition will execute when the if condition gets input as "false". else keyword will be executing when if condition and every elif condition gets input as "false". 

```

</br>

<b> Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote". </b>

```
age = int(input("Enter age"))
if age >= 18:
    print("I can vote")
else:
    print("I can't vote")

```

<b> Q23. Write a code that displays the sum of all the even numbers from the given list. </b>
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
```
numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for number in numbers:
    if number % 2 == 0:
        sum+=number
```

<b> Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output. </b>
-> 
```
a,b,c = input("Enter number").split(" ")
sum = int(a) + int(b) + int(c)

```

<b> Q25. Write a program to display only those numbers from a list that satisfy the following conditions </b>

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop

```
numbers = [12, 75, 150, 180, 145, 525, 50]
for number in numbers:
    if number % 5 == 0 and number <= 150:
        print(number)
    elif number > 150:
        break
```

<b> Q26. What is a string? How can we declare string in Python? </b>

</br>

```
-> string is collection of characters which can be simply declared by enclosing sequence of characters into quotes, double quotes or triple quotes
```

</br>

<b> Q27. How can we access the string using its index? </b>
```
-> string can be access by passing index into square brackets
```

</br> 

<b> Q28. Write a code to get the desired output of the following </b>
```
string = "Big Data iNeuron"
desired_output = "iNeuron"

```
```
string = "Big Data iNeuron"
string.split()[-1]  # accessing the last word of string
```

</br> 


<b> Q29. Write a code to get the desired output of the following </b>

```
string = "Big Data iNeuron"
desired_output = "norueNi"


```

```
string = "Big Data iNeuron"
string.split()[-1::-1][::-1]  # accessing the last word of string and reversing the last word

```

</br> 


<b> Q30. Resverse the string given in the above question. </b>
```
string = "Big Data iNeuron"
string.split()[::-1]  # reversing the string given in the above question
```

</br> 


<b> Q31. How can you delete entire string at once? </b>
```
-> string can be deleted through del keyword
```

<b> Q32. What is escape sequence? </b>

```
an escape sequence is a sequence of characters that represents a special character, such as a newline or a tab. Escape sequences are often used in strings to represent characters that cannot be typed directly, or to represent characters that have a special meaning in the context of the string.
```

 </br>


<b> Q33. How can you print the below string? </b>


```
'iNeuron's Big Data Course'
```


```
print(iNeuron\'s Big Data Course)
```

</br>


<b> Q34. What is a list in Python? </b>

```
-> list is mutable collection of objects separated by commas and enclosed between square brackets.
```


<b> Q35. How can you create a list in Python? </b>

```
-> list can be created by enclosing values between square brackets and seprated by comma.
```

</br>


<b> Q36. How can we access the elements in a list? </b>

```
-> elements in list can be accessed by passing index of element in square brackets.
```


<b> Q37. Write a code to access the word "iNeuron" from the given list. </b>
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
print(lst[4][2])
``` 

<b> Q38. Take a list as an input from the user and find the length of the list. </b>
-> 

```
arr = input("enter array seprated by spaces")
len_arr = len(arr.split(" "))
print(len_arr)

```

<b> Q39. Add the word "Big" in the 2rd index of the given list. </b>

```
lst = ["Welcome", "to", "Data", "course"]
lst.insert(2,"big")
print(lst)

```

<b> Q40. What is a tuple? How is it different from list? </b>
```
-> tuple is immutable collection of objects separated by commas. tuple is simmilar to list in terms of slicing and indexing however we can not modify tuple like list.

- list acts as dynamic array where as tuple acts as fixed array.


```

<b> Q41. How can you create a tuple in Python? </b>
```
-> tupple can be created by passing comma separated values in brackets 
```

</br>

<b> Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason. </b>

-> yes we can add name to the tuple by concatinating tuples
```
tpl = (1,2,3)
tpl2 = ('sahil',None)

print(tpl + tpl2[0:1])
```


<b> Q43. Can two tuple be appended. If yes, write a code for it. If not, why? </b>
yes we can 
```
tpl = (1,2,3)
tp2 = ('sahil',"")

print(tpl1 + tpl2[0:1])
```


<b> Q44. Take a tuple as an input and print the count of elements in it. </b>

```
tpl = (1,2,3)
print(len(tpl))

```

<b> Q45. What are sets in Python? </b>
```
-> A Set is an mutable unordered collection data which does not have duplicate elements. 

- Set are represented by { } (values enclosed in curly braces)

- This is based on a data structure known as a hash table

- Since sets are unordered, we cannot access items using indexes as we do in lists.
 
```

<b> Q46. How can you create a set? </b>
```
-> set can be created by enclosing value in curly brackets.

```

<b> Q47. Create a set and add "iNeuron" in your set. </b>
 

```

empty_set = set()
empty_set.add("iNeuron")

```

<b> Q48. Try to add multiple values using add() function. </b>
```
st1 = set()
st2 = {1,2,3,4} # or lst = [1,2,3,4]
st1.update(lst)
print(st1)

```

<b> Q49. How is update() different from add()? </b>
```
-> update is used to add multiple elements in set where as add is used tos add single element in set

```

<b> Q50. What is clear() in sets? </b>
```
-> clear() is used to remove all the elements from set.
```

<b> Q51. What is frozen set? </b>
```
-> frozen set is immutable object in python. This means that once a frozen set has been created, its elements cannot be added, removed, or changed. Frozen sets are useful for situations where you need to store a set of values that should not be changed.
```

<b> Q52. How is frozen set different from set? </b>
```
=> The main difference between sets and frozen sets in the Python programming language is that sets are mutable, while frozen sets are immutable. This means that sets can be modified after they are created, while frozen sets cannot be modified.
```

<b> Q53. What is union() in sets? Explain via code. </b>
```
-> Union is function of set that returns new set where elements of both the set are present 
```

```
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

union_set = set1.union(set2)

print(union_set)  # Output: {1, 2, 3, 4, 5, 6}
```

<b> Q54. What is intersection() in sets? Explain via code. </b>
```
-> intersection is a function in set that returns new set which contains only elements which are present in both the sets.
```
```
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

intersection_set = set1.intersection(set2)

print(intersection_set)  # Output: {3, 4}
```
<b> Q55. What is dictionary ibn Python? </b>
```
-> dictionary is data type in python which stores key-value pairs. A dictionary is similar to a list or an array, but instead of storing a sequence of values, it stores a collection of values that are accessed using keys. Each key-value pair in a dictionary is known as an item.
```
<b> Q56. How is dictionary different from all other data structures. </b>
```
A dictionary is different from other data structures in Python because it stores its data as a collection of key-value pairs instead of a sequence of values. This means that you can access the items in a dictionary using keys, which are unique identifiers for each item in the dictionary. Other data structures, such as lists and arrays, store their data as a sequence of values, which means that you can access the items in those data structures using indices.

Another important difference between dictionaries and other data structures is that the items in a dictionary are not ordered. In other words, the items in a dictionary do not have a specific position or index. This means that you cannot access the items in a dictionary using an index, like you can with other data structures. Instead, you must use the corresponding key for each item to access its value.

```

<b> Q57. How can we delare a dictionary in Python? </b>
```
To create a dictionary in Python, you can use the dict() constructor or the {} notation. 
```

<b> Q58. What will the output of the following? </b>
```
var = {}
print(type(var))
```
```
#Output: <class 'dict'>
```

<b> Q59. How can we add an element in a dictionary? </b>
```
To add an element to a dictionary in Python, you can use the square bracket notation to specify the key for the new element, and assign a value to that key. 
```

Q60. Create a dictionary and access all the values in that dictionary.
```
-> to access all the values in the dictionary we can use values() function
```
```
my_dict = {
    "name": "sahil",
    "age": 19,
    "city": "Surat"
}

values = my_dict.values()

print(values) 
```
<b> Q61. Create a nested dictionary and access all the element in the inner dictionary. </b>
```
my_dict = {
    "name": "sahil",
    "age": 19,
    "city": "Surat"
}
outer_dict = {
    "inner_dict1" : my_dict,
    "inner_dict2" : my_dict
}

for key in outer_dict:
    inner_dict_val = outer_dict[key]
    for dict_key in inner_dict_val:
        print(inner_dict_val[dict_key])

```

<b> Q62. What is the use of get() function? </b>
```
In Python, the get() method is used to return the value of a specified key in a dictionary. If the key does not exist, the get() method can return a default value or None, depending on how it is called. Here is an example of how to use the get() method
```

<b> Q63. What is the use of items() function? </b>
```
The items() method returns a view object. The view object contains the key-value pairs of the dictionary, as tuples in a list.


```

<b> Q64. What is the use of pop() function? </b>
```
 the pop() function is used to remove an item from a dictionary and return its value
```

<b> Q65. What is the use of popitems() function? </b>
```
The popitem() method removes the item that was last inserted into the dictionary. 
```

<b> Q66. What is the use of keys() function? </b>
```
keys() is function that returns the dynamic view of the dictionary keys that we can itterate over.
```

<b> Q67. What is the use of values() function? </b>
```
values() is function that returns the dynamic view of the dictionary values that we can itterate over.
```

<b> Q68. What are loops in Python? </b>
```
In Python, a loop is a control flow statement that allows you to repeat a block of code a certain number of times or until a certain condition is met. There are two types of loops in Python: for loops and while loops.
```

<b> Q69. How many type of loop are there in Python? </b>
```
There are two type of loops in Python 
1. For loop
2. While loop
```

<b> Q70. What is the difference between for and while loops? </b>
```
The main difference between a for loop and a while loop is the way they are used. A for loop is used to iterate over a sequence of elements, such as a list or a string. This means that the loop will run once for each element in the sequence, and the variable used to refer to each element will take on the value of each element in turn. In contrast, a while loop is used to repeatedly execute a block of code as long as a certain condition is met. This means that the loop will continue to run until the condition is no longer met, and the variable used to track the condition can be updated in the body of the loop.
```

<b> Q71. What is the use of continue statement? </b>
```
continue statement is used inside the loops and this statment will skip the current itteration
```

<b> Q72. What is the use of break statement? </b>
```
break statement is used inside the loops and this statment will terminate the loop
```
<b> Q73. What is the use of pass statement? </b>
```
The pass statement is a null statement in Python, which means that it does nothing. It is used as a placeholder in situations where a statement is required syntactically, but no action needs to be performed

```

<b > Q74. What is the use of range() function? </b>
```
The range() function is a built-in function in Python that returns a sequence of numbers. function takes three arguments: start, stop, and step.
```

Q75. How can you loop over a dictionary?
```
To loop over a dictionary you can pass a dictionary to the for loop, there are two ways it can be Done.
First way is to use keys() function. and other way is to use without key function.

# without key function

    for key in my_dict:
      a = key
#with key function
    for key in my_dict.keys():
      a = key

both the thing are same in python 3, they returns dict_keyiterator. 

print(type(iter({})))
 # op : <class 'dict_keyiterator'>
print(type(iter({}.keys())))
 # op : <class 'dict_keyiterator'>

 however there's additional negligable cost of function call in keys() method.
```


### Coding problems
<b> Q76. Write a Python program to find the factorial of a given number. </b>
```
fact = 1
num = 10
while num > 1:
    fact *= num
    num -= 1
```
<b> Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100 </b>+cwh
```
a,b,c = input("Enter value of p r t in sequence")
si = (float(p) * float(r) * float(t)) /100

print("simple interest is ",si)

```

<b> Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t. </b>
```
a,b,c = input("Enter value of p r t in sequence")

a = float(p)((1 + float(r))/100 ) ** float(t)

print("compound interest is ",a)

```

<b> Q79. Write a Python program to check if a number is prime or not. </b>
```
num = int(input("enter number"))

flag = "false"
if num == 4:
    flag = "true"
for i in range(2,int(num/2)):
   
    if num % i == 0 :
        flag = "true"
        break
if flag:
    print("number is prime")
else:
    print("number is not prime")

```

<b> Q80. Write a Python program to check Armstrong Number. </b>
```
num = int(input("enter number"))
sum = 0
for digit in str(num):
    sum += int(digit) ** 3

if sum == num:
    print("number is Armstrong")
else:
    print("number is not Armstrong")

```

<b> Q81. Write a Python program to find the n-th Fibonacci Number. </b>

```
num = int(input("enter number"))
if n == 1:
    print("0")
elif n == 2:
    print("1")
elif n <0:
    print("envalid input")
    exit()

current = 1 
prev = 0
cursor = 2
while cursor < n:
    next = current + prev
    prev = current 
    current = next
    print(current)
    cursor += 1
```

<b> Q82. Write a Python program to interchange the first and last element in a list. </b>
```
lst = [1,2,3,4,5]
temp = lst[0]
lst[0] = lst[-1]
lst[-1] = temp
```

Q83. Write a Python program to swap two elements in a list.
```
lst = [1,2,3,4,5]
n,m = input("enter nth and mth location to swap in dictionary").split(" ")
n = int(n)
m  = int(m)
if n >= len(lst) or m >= len(lst):
    print("index out of range")
    exit()
temp = lst[n-1]
lst[n-1] = lst[m-1]
lst[m-1] = temp

print(lst)
```

Q84. Write a Python program to find N largest element from a list. # prepare sorting algorithms 
```
def sort_arr(arr, n):

    if n > len(arr):
       return "[ERROR]  N greater then array length"
        

    for i in range(n):
        for j in range(len(arr)-i-1):
            if arr[j] > arr[j+1]:
                temp = arr[j] 
                arr[j] = arr[j+1]
                arr[j+1] = temp
    return arr[-1:-1*(n+1):-1]


sort_arr(arr,5)
```

Q85. Write a Python program to find cumulative sum of a list.
```
def cumulative_sum(numbers):
  cum_sum = []
  for i, num in enumerate(numbers):
    if i == 0:
      cum_sum.append(num)
    else:
      cum_sum.append(cum_sum[i-1] + num)
  return cum_sum

print(cumulative_sum([1, 2, 3, 4]))

```
Q86. Write a Python program to check if a string is palindrome or not.

```
string = "Big Data iNeuron"
print("is palindrome : ", string == string[::-1])
```

Q87. Write a Python program to remove i'th element from a string.
```
s = 'sahil'
i = 2
if i<0 or i > len(s):
    print("invalid number") 

s = i[:n-1] + i[n:]
print(s)

```

Q88. Write a Python program to check if a substring is present in a given string.
```
string = "sahil"
sub = 'sa'

print("sub string present : " sub in string)

```
Q89. Write a Python program to find words which are greater than given length k.

```
text = "The quick brown fox jumped over the lazy dog"

k = 4

words = text.split()

for word in words:
    if len(word) > k:
        print(word)

```


Q90. Write a Python program to extract unquire dictionary values.
```
dictt = {
    "a" : 1,
    "b" : 1,
    "c" : 2,
}
unique_vals = set(dictt.values())
print(unique_vals)
```

Q91. Write a Python program to merge two dictionary.
```
dictt2 = {
    "d" : 1,
    "e" : 1,
    "f" : 2,
}

dictt1 = {
    "a" : 1,
    "b" : 1,
    "c" : 2,
}

dict1.update(dictt2)
print(dict1)
```
Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
```
lst = [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]

dct = {}

for tup in lst:
  dct[tup[0]] = tup[1]

print(dct)

```
Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```

```
lst = [9, 5, 6]

result = []

for num in lst:
  tpl = (num, num**3)
  result.append(tpl)

print(result)

```



Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
```
test_tuple1 = (7,2)
test_tuple2 = (7, 8)
lst = []
for i in test_tuple1:
    for j in test_tuple2:
        lst.append((i,j))
        lst.append((j,i))

```

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```

```
ar = [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
for i in range(1,len(ar)):
    for j in range(len(ar) - i):
        if ar[j][1] > ar[j+1][1]:
            temp = ar[j] 
            ar[j] = ar[j+1]
            ar[j+1] = temp


```



Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
```
n = 5
for i in range(n):
    for j in range(i + 1):
        print("*",end=" ")
    print("")
```
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
```
n = 5
for i in range(n):
    space_count = n - i - 1
    for j in range(space_count):
        print(" ",end="")

    number_stars = n - space_count
    for j in range(number_stars):
        print("*",end="")
    print("")

```
Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
```
n = 5
for i in range(n):
    space_count = n - i - 1
    for j in range(space_count):
        print(" ",end="")

    number_stars = n - space_count
    for j in range(number_stars):
        print("*",end=" ")
    print("")

```



Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
```
n = 5
for i in range(n):
    for j in range(1,i+2):
        print(j,end=" ")
    print("")+
```
Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
```
n = 5
for i in range(n):
    selected_char = chr(65 + i)

    for j in range(i+1):
        print(selected_char,end = " ")
    print("")

```

