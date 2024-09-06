# Python Programming tutorial

# Note!

### This tutorial is for those who are already familiar with programming, and want to learn python. I will try to make this course as easy as possible Inshaa Allah.

## Installation

To get started with installation you have to follow these steps:

## Step 1 : Downlaod the interpreter.

### Step 1.1

### Go to [python.org](https://www.python.org/downloads/) and click on download button to install latest interpreter.

![alt text](image.png)

During Installation it asks for an option _add interpreter to path_ or _add .bin folder to path_ something like this. Make sure to check this option.

### Step 1.2

Once it's installed open your VS code or any other IDE, create a file with name **new.py**

in file write following line of code.

```Python
print('I am running')
```

### Step 1.3

if you have [code runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) extention installed run the file to print **I am running**.

### Step 1.4

If this doesnot work it probably means your enviroment varaibles in path are not properly set, or you are not running it properly.
In that case follow this page to setup environment variables [Set environment variables for python](https://realpython.com/add-python-to-path/)

**Note : ** you don't need this step if you follow step 1.1 correctly, and your program is running, this step is to make program running.

## Step 2

## Learn About Python

## Step 3

## Learn Python

### Step 3.1

## Input and Output.

### Output

```Python
print('simple print statement like this displays output on screen')
```

### Input

```Python
input('simple input statement like this displays the text on screen and wait for user to input any thing(number or string)')
```

### Step 3.2

## Variables

Above we have inputed the data and doesn't store it into any variable, so you might run into problems while running above code.

# Corrected Code

```Python
str = input('This time the input will store into the variable str')
```

### Note : Python always by default take input as strings, to take integers as input are defined in seciton Datatypes.

## **What are Variables**

Varables are like containers in memory that stores the data, as you are already familiar with. So in python there is no need of declaration of variables seperately as in other programming languages. you can just initialize it like that.

```Python
num = 10
```

To initialize variable will null we use keyword none in python.

```Python
num = none
```

### Step 3.2

## **DataTypes(Primitive Datatypes)**

Every variable in python also has datatype as in any other language but the main differnce is, it provides alot of flexibility becuase you don't have to mention datatype explicitly, as our interpreter understands the datatype on its own.

### Example

```Python
num = '12'
```

Here above num has datatype string so our interpreter is already aware of it.

```Python
num = 12
```

Here above num has datatype integer so our interpreter is already aware of it because it is written without quotes.

## Strings

String variables are those variables in which data has single quotes _''_ or double quotes _""_ about it

## **Valid Examples**

```Python
my_str = 'It is a string with single quotes'
```

```Python
my_str = "It is a string with double quotes"
```

Numbers can be string when surrounded by quotes.

```Python
my_str = '12'
```

## **Invalid Examples**

```Python
my_str = 'It is a Invalid because starting and ending quotes type mismatched"
```

## _Recommended_

It is recommended to use single quotes when using double quotes inside, and using double quotes around if using single inside.

### **Example**

```Python
my_str = "It's my book"
```

```Python
my_str = 'He said : "It\'s my book"'
```

In cases like above we have to use [escape sequences](https://www.scaler.com/topics/escape-sequence-in-python/)

### _[escape sequences](https://www.scaler.com/topics/escape-sequence-in-python/) are used for special type of characters in strings like \n for new line, \t for tab spaces etc_

## **Integers**

Integer datatype is used to represent numbers, a string number is not equal to a integer number.

```Python
'23' == 23 // False
'23' == '23' // True
23 == 23 // True
```

### **Note** : Operators like +, -, \*, / are applied to both integers and strings but thier usecases are different in both.

## **DataTypes(Non Primitive Datatypes)**

## **Lists**

List are an example of non primitive data types, because these are the combinations of primitive datatypes.

Like in C/C++ we have an array, that is the collection of homogenous data items at one place, and accessed through index.

Similarly in python, they can be accessed by indices, but they are collection of non homogenous data items or homogenous data items depending on our preference.

### **Example**

```Python
my_list = ['Ebad-ur-Rehman', 20, 'Computer Science']
```

This is completely valid in python to include integers strings, and even other datatypes like sets, dictionaries, and tuples within a list.(I will discuss about other datatypes later.)

### Accessing through indices.

```Python
my_list = ['Ebad-ur-Rehman', 20, 'Computer Science']
print(my_list[0]) // displays Ebad-ur-Rehman on console
print(my_list[1]) // displays 20 on console
print(my_list[2]) // displays Computer Science on console
```

### Adding new Elements

**At last of List**

```Python
my_list.append('AI')
print(my_list) // ['Ebad-ur-Rehman', 20, 'Computer Science' ,'AI']
```

**Anywhere**

```Python
// inserting at 0 index
my_list = ['Ebad-ur-Rehman', 20, 'Computer Science']
my_list.insert(0, 'AI')
my_list = ['AI', 'Ebad-ur-Rehman', 20, 'Computer Science']
```
