# PYTHON FUNCTIONS (Assg:4)

### 1. What does the len() function do in Python? Write a code example using len() to find the length of a list.

#### The len() function in Python is used to determine the number of elements in a data structure such as a list, tuple, dictionary, or string. It returns an integer representing the total number of items.

##### PROGRAM-1

list=[2,4,6,8]   # CREATING A SIMPLE LIST

length=len(list) # FINDING THE LENGTH OF THE LIST

print("The length of the list ", list, "is :", length) # DISPLAYING THE RESULT


##### OUTPUT-1

![image](https://github.com/user-attachments/assets/54f97870-d196-4fb2-8600-12b6a289333d)



### 2. Write a Python function greet(name) that takes a person's name as input and prints "Hello, [name]!".

##### PROGRAM-2

def greet(name):   # DEFINING THE GREETING FUNCTION
    print(f"Hello, {name}!")

#EXAMPLE USAGE
greet("Liana")


##### OUTPUT-2

![image](https://github.com/user-attachments/assets/492036f4-87fc-4969-92ce-761a6cb84093)



### 3. Write a Python function find_maximum(numbers) that takes a list of integers and returns the maximum value without using the built-in max() function. Use a loop to iterate through the list and compare values.


##### PROGRAM-3

def find_maximum(numbers):

    if not numbers:
    
        return None
        
       
    maxvalue=numbers[0]
    
        
    for num in numbers:
    
        if num>maxvalue:
        
            maxvalue=num
   
    return maxvalue
                
numbers=[8,7,3,10,23,6]

result=find_maximum(numbers)

print(f"The maximum value in the list is : {result}")


##### OUTPUT-3

![image](https://github.com/user-attachments/assets/831cf8b1-5c62-4c6a-9192-87e7f0bc4a97)



### 4. Explain the difference between local and global variables in a Python function. Write a program where a global variable and a local variable have the same name and show how Python differentiates between them.


![image](https://github.com/user-attachments/assets/6da38fee-faba-416f-81d3-dd48b135b7a6)


##### PROGRAM-4


message="I am the Global Variable"

def local():

    message="I am the Local Variable"
    
    print("Inside the function:",message)

def modify_global():

    global message
    
    message="I am the modified Global Variable"

local()

print("Outside the function:",message)

modify_global()

print("After modifying the variable:",message)



##### OUTPUT-4

![image](https://github.com/user-attachments/assets/658c29fd-91ea-491c-bc6a-4c02fbbce337)


### 5. Create a function calculate_area(length, width=5) that calculates the area of a rectangle. If only the length is provided, the function should assume the width is 5. Show how the function behaves when called with and without the width argument.


##### PROGRAM-5


def calculate_area(length,width=5):

    return length*width

area1=calculate_area(10,8)

print("The area without width argument is:",area1)


area2=calculate_area(10)

print("The area with width argument as 5 by default is:",area2)


##### OUTPUT-5

![image](https://github.com/user-attachments/assets/9c635a32-9cc7-4e02-a436-4030627e5781)







