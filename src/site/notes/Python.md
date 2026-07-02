---
{"dg-publish":true,"permalink":"/python/","tags":["gardenEntry"],"dg-note-properties":{}}
---

dg-publish:  true



# 1. Printing Something 

**Syntax** : <nobr> print(oper_1 Operand oper_2) </nobr>

print(5-8) → -3
print(5+8)
print(5×8)
print(8/8)
print(5%8)

Formula:
BMI = Weight / (height)^²   

Method-1
BMI =    W / h ** 2
Method-2
BMI = w/(h×h)

# 2. Checking Type

**Syntax** : type(var_name)

type(BMI)

# 3. Python list
Name of collection of values.
1. Can have different types.
**Syntax** : [a,b,c,d,e,...]
I)
[1.0., 3.7, 4.6, 3.6]
family = [1.0., 3.7, 4.6, 3.6]

II)
**Input** : 
["CCC", 6.0, "ATYR", 1.4, "FSYY", 3.4]
fam = ["CCC", 6.0, "ATYR", 1.4, "FSYY", 3.4]
**Output** : ['CCC', 6.0, 'ATYR', 1.4, 'FSYY', 3.4]

III)list within list
fam2 = [ ["Luzi", 1.45], ["Ahah", 1.35], ["Dyer", 5.4] ]

# 4. list Type

**Input** : type(fam)
**Output** : list

# 5. Sub-setting lists

**Accessing 6th(last) element** : fam[5] → same
**Accessing 6th(last) element by -ve number** : fam[-1] → same

# 6. list Slicing

**Syntax** : <nobr>list_name[Starting_point : Excluding_point] </nobr>

**Input** : fam[2:4] → 3rd list will display and others are not.
**Output** : ['ATYR', 1.4]

fam[:4]
['CCC', 6.0, 'ATYR', 1.4]

# 7. Changing list Elements

I)
fam[5] = 1.7
II)
fam[0:2] = ["Lis", 1.55 ]

# 8. Adding and Removing elements

###### Adding
**Input** : 
fam + ["me", 1.3]
fam = ["CCC", 6.0, "ATYR", 1.4, "FSYY", 3.4, "me", 1.3]
fam_ext = fam + ["me", 1.3]
###### Removing
del fam[2]
fam 

# 9. Assigning list 

###### 1. Assignment method
**Changes in y will make change in fam also.**
y = fam
y[1] = "z"

###### 2. List Function
**Changes in y will make not change in fam.**
y = **list**(fam)
Now, this will not work.
y = fam
fam
###### 3. List Slicing
y = fam[:]

# 10. Functions

1. *Syntax*: 
###### **max**(list_name)
tallest = **max**(fam)
tallest

2. *Syntax_1* : 
###### **round**(decimal_no, decimal_place)
Input : **round**(1.68, 1)
Output : 1.7

*Syntax_2* :
###### **round**(decimal_no)
Input : **round**(1.68)
Output : 2

3. *Syntax* :
###### **help**(other_functions_name)
Input : **help**(round)
Output : Some Info.

4. *Syntax* :
###### **?** other_functions_name
Input : **?** round
Output : Some Info.

# 11. Methods
Functions that belongs to **Objects(everything)** such as int, float, str, list; etc.
Different types of Objects can have same method name.
e.g.  
For **string** : sister.**index**("z" )
For **list** : fam.**index**("mom")

Input :
fam.**append**("me")
fam
Output : 
["CCC", 6.0, "ATYR", 1.4, "FSYY", 3.4, "me", 1.3, 'me']
## i. list methods
*Syntax* : 
Object_name.**method_name**(argu.)
1. **index()** → For string
Input : fam.**index**("ATYR" )
Output : 2

2. **count()** → For integers
Input : fam.**count**(6.0)
Output : 1

## i. str methods
*Syntax* : 
Object.**method_name**()
1. **capitalize**()
Input : 
sister = "liz"
sister.**capitalize**()
Output : 'Liz'

2. **replace**("Replace_word", "Add_word" )
Input : sister.**replace**("z", "sa")
Output : 'lisa'

# 12. numpy
https://plp.pypa.lo/en/stable/Installation/
**Download** : get–pip.py
**Terminal** :
python3 get–pip.py
pip3 install numpy
**Import** :
1. import numpy
2. import numpy as np
3. from numpy import array

*Syntax* :

1. numpy.array([1,2,3])
2. np.array([1,2,3]) → recommended 
3. array([1,2,3])