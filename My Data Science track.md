
## PYTHON CODING ##

Python is perfectly suited to do basic calculations. Apart from addition, subtraction, multiplication and division, there is also support for more advanced operations such as:

Exponentiation: **. This operator raises the number to its left to the power of the number to its right. For example 4**2 will give 16.
Modulo: %. This operator returns the remainder of the division of the number to the left by the number on its right. For example 18 % 7 equals 4.

In the previous exercise, you worked with two Python data types:

int, or integer: a number without a fractional part. savings, with the value 100, is an example of an integer.

float, or floating point: a number that has both an integer and fractional part, separated by a point. growth_multiplier, with the value 1.1, is an example of a float.
Next to numerical data types, there are two other very common data types:

str, or string: a type to represent text. You can use single or double quotes to build a string.

bool, or boolean: a type to represent logical values. Can only be True or False (the capitalization is important!).

#### TYPES OF VALUES OR VARIABLES ####
To find out the type of a value or a variable that refers to that value, you can use the type() function. Suppose you've defined a variable a, but you forgot the type of this variable. To determine the type of a, simply execute:

type(a)
 And this would be a string.

 **Type conversion** 
 
Using the + operator to paste together two strings can be very useful in building custom messages.

Suppose, for example, that you've calculated the return of your investment and want to summarize the results in a string. Assuming the integer savings and float result are defined, you can try something like this:
```
print("I started with $" + savings + " and now have $" + result + ". Awesome!")

```
This will not work, though, as you cannot simply sum strings and integers/floats.

To fix the error, you'll need to explicitly convert the types of your variables. More specifically, you'll need str(), to convert a value into a string. str(savings), for example, will convert the integer savings to a string.

Similar functions such as int(), float() and bool() will help you convert Python values into any type.

 correcting a wrong code using PYTHON

 **Definition of savings and result**
 
 ```
savings = 100
result = 100 * 1.10 ** 7

```

**Fix the printout**

```
print("I started with $" + savings + " and now have $" + result + ". Awesome!")

```
**Definition of pi_string**
```
pi_string = "3.1415926"

```
#### Convert pi_string into float: pi_float ####

ANSWER

**Definition of savings and result**
```
savings = 100
result = 100 * 1.10 ** 7

```
**Fix the printout**
```
print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

```
**Definition of pi_string**
```
pi_string = "3.1415926"

```
**Convert pi_string into float: pi_float***
```
pi_float = float(pi_string)

```
# LISTS#
A list is a way to give a single name to a collection of values.

Create a list, areas, that contains the area of the hallway (hall), kitchen (kit), living room (liv), bedroom (bed) and bathroom (bath), in this order. Use the predefined variables.
Print areas with the print() function.

EXAMPLE
**Area variables (in square meters)**
```
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

```
**Create list areas**
```
areas = [hall, kit, liv, bed, bath]

```
**Print areas**
```
print(areas)
[11.25, 18.0, 20.0, 10.75, 9.5]

```
### Create list with different types ###
A list can contain any Python type. Although it's not really common, a list can also contain a mix of Python types including strings, floats, booleans, etc.

**area variables (in square meters)**
```
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

```
**Adapt list areas**
```
areas = ["hallway", hall, "kitchen", kit, "living room", liv, "bedroom", bed, "bathroom", bath]

```
The code in the editor is the start of a solution. For some of the areas, the name of the corresponding room is already placed in front. Pay attention here! "bathroom" is a string, while "bath" is a variable that represents the float 9.50 you specified earlier.

Finish the code that creates the areas list. Build the list so that the list first contains the name of each room as a string and then its area. In other words, add the strings "hallway", "kitchen" and "bedroom" at the appropriate locations.
Print areas again; is the printout more informative this time?

 **SOLUTION**
Area variables (in square meters)

```
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

```
**Adapt list areas**
```
areas = ["hallway", hall, "kitchen", kit, "living room", liv, "bedroom", bed, "bathroom", bath]

```
#### Print areas ####
```
print(areas)
['hallway', 11.25, 'kitchen', 18.0, 'living room', 20.0, 'bedroom', 10.75, 'bathroom', 9.5]

```

**List of lists**

As a data scientist, you'll often be dealing with a lot of data, and it will make sense to group some of this data.

Instead of creating a flat list containing strings and floats, representing the names and areas of the rooms in your house, you can create a list of lists. The script in the editor can already give you an idea.

**area variables (in square meters)**
```
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

```

**house information as list of lists**
```
house = [["hallway", hall],
         ["kitchen", kit],
         ["living room", liv],
         ["bedroom", bed],
         ["bathroom", bath]]
         
```         

Print out house
```
print(house)

```
#### SOLUTION ####
```
[['hallway', 11.25], ['kitchen', 18.0], ['living room', 20.0], ['bedroom', 10.75], ['bathroom', 9.5]]

```
Print out the type of house
```
print(type(house))

[['hallway', 11.25], ['kitchen', 18.0], ['living room', 20.0], ['bedroom', 10.75], ['bathroom', 9.5]]
<class 'list'>

```
**Subset and conquer**

Subsetting Python lists is a piece of cake. Take the code sample below, which creates a list x and then selects "b" from it. Remember that this is the second element, so it has index 1. You can also use negative indexing.

```
x = ["a", "b", "c", "d"]
x[1]
x[-3] # same result!

```
** Remember the areas list from before, containing both strings and floats? Its definition is already in the script. Can you add the correct code to do some Python subsetting?***

### EXAMPLE ###

**Create the areas list**
```
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

```
Print out the second element from the areas list (it has the value 11.25).
Subset and print out the last element of areas, being 9.50. Using a negative index makes sense here!
Select the number representing the area of the living room (20.0) and print it out.

**Print out second element from areas**
```
print(areas[1])

```
**Print out last element from areas**
```
print(areas[-1])

```
**Print out the area of the living room**
print(areas[5])


#### RESULT ####
11.25
9.5
20.0

**Subset and calculate**

After you've extracted values from a list, you can use them to perform additional calculations. Take this example, where the second and fourth element of a list x are extracted. The strings that result are pasted together using the + operator:
```

x = ["a", "b", "c", "d"]
print(x[1] + x[3])

```

**Create the areas list**
```
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]
```

**Sum of kitchen and bedroom area: eat_sleep_area**
**Print the variable eat_sleep_area**
```
eat_sleep_area = areas[3] + areas[-3]
print(eat_sleep_area)

```
**solution**
```
28.75

<script.py> output:
    28.75
    
```
### Slicing and dicing ###
Selecting single values from a list is just one part of the story. It's also possible to slice your list, which means selecting multiple elements from your list. Use the following syntax:

```
my_list[start:end]

```
The start index will be included, while the end index is not.

The code sample below shows an example.
```
A list with "b" and "c", corresponding to indexes 1 and 2, are selected from a list x:

x = ["a", "b", "c", "d"]
x[1:3]

```
The elements with index 1 and 2 are included, while the element with index 3 is not.

Use slicing to create a list, downstairs, that contains the first 6 elements of areas.
Do a similar thing to create a new variable, upstairs, that contains the last 4 elements of areas.
Print both downstairs and upstairs using print().

**ANSWER**

**Create the areas list**
```
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]
```

**Use slicing to create downstairs**
```
downstairs = areas[0:6]
```

**Use slicing to create upstairs**
```
upstairs = areas[6:10]
```
Print out downstairs and upstairs
```
print(downstairs)
print(upstairs)
```

Answer
['hallway', 11.25, 'kitchen', 18.0, 'living room', 20.0]
['bedroom', 10.75, 'bathroom', 9.5]

# MANIPULATING LISTS #

Replace list elements
Replacing list elements is pretty easy. Simply subset the list and assign new values to the subset. You can select single elements or you can change entire list slices at once.

Use the IPython Shell to experiment with the commands below. Can you tell what's happening and why?

```
x = ["a", "b", "c", "d"]
x[1] = "r"
x[2:] = ["s", "t"]

```
For this and the following exercises, you'll continue working on the areas list that contains the names and areas of different rooms in a house.

```
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]
```
Update the area of the bathroom area to be 10.50 square meters instead of 9.50.

ANSWER
```
areas[9] = 10.50

```
Make the areas list more trendy! Change "living room" to "chill zone".
```
areas[4] = "chill zone"

```

***Extend a list***

If you can change elements in a list, you sure want to be able to add elements to it, right? You can use the + operator:

```
x = ["a", "b", "c", "d"]
y = x + ["e", "f"]
```
```
areas = ["hallway", 11.25, "kitchen", 18.0, "chill zone", 20.0,
         "bedroom", 10.75, "bathroom", 10.50]
```
### PRACTICE ###
Use the + operator to paste the list ["poolhouse", 24.5] to the end of the areas list. Store the resulting list as areas_1.

```
areas_1 = areas + ["poolhouse", 24.5]

```

Further extend areas_1 by adding data on your garage. Add the string "garage" and float 15.45. Name the resulting list areas_2.

```
areas_2 = areas_1 + ["garage",15.45]

```
**Delete list elements**

Finally, you can also remove elements from your list. You can do this with the ``` del ``` statement:
```
x = ["a", "b", "c", "d"]
del(x[1])

```

Pay attention here: as soon as you remove an element from a list, the indexes of the elements that come after the deleted element all change!

The updated and extended version of ``` areas ``` that you've built in the previous exercises is coded below. You can copy and paste this into the IPython Shell to play around with the result.

```
areas = ["hallway", 11.25, "kitchen", 18.0,
        "chill zone", 20.0, "bedroom", 10.75,
         "bathroom", 10.50, "poolhouse", 24.5,
         "garage", 15.45]
         
```

There was a mistake! The amount you won with the lottery is not that big after all and it looks like the poolhouse isn't going to happen. You decide to remove the corresponding string and float from the ``` areas``` list.

The ``` ; ```sign is used to place commands on the same line. The following two code chunks are equivalent:

```
Same line
command1; command2

Separate lines
command1
command2
```
# FUNCTIONS #

#### Familiar functions ####

Out of the box, Python offers a bunch of built-in functions to make your life as a data scientist easier. You already know two such functions: ``` print() ``` and ``` type() ```. You've also used the functions ``` str() ```, ``` int() ```, ``` bool() ``` and ``` float() ``` to switch between data types. These are built-in functions as well.

Calling a function is easy. To get the type of ``` 3.0 ``` and store the output as a new variable, result, you can use the following:

``` result = type(3.0) ```

The general recipe for calling functions and saving the result to a variable is thus:

``` output = function_name(input) ```

**EXAMPLE**

```
var1 = [1, 2, 3, 4]
var2 = True
```

Use ``` print() ``` in combination with ``` type() ``` to print out the type of var1.

```
print(type(var1))
```

Use ``` len() ``` to get the length of the list ``` var1 ```. Wrap it in a ``` print() ``` call to directly print it out.

```
print(len(var1))
```

Use ``` int() ``` to convert ``` var2 ``` to an integer. Store the output as ``` out2. ```

```
out2 = int(var2)
```

### Help! ###

Maybe you already know the name of a Python function, but you still have to figure out how to use it. Ironically, you have to ask for information about a function with another function: ``` help(). ``` In IPython specifically, you can also use ``` ? ``` before the function name.

To get help on the ``` max() ``` function, for example, you can use one of these calls:

```
help(max)
?max

```

**Multiple arguments**

In the previous exercise, you identified optional arguments by viewing the documentation with ``` help().``` You'll now apply this to change the behavior of the ``` sorted() ``` function.

Have a look at the documentation of ``` sorted() ``` by typing ``` help(sorted) ``` in the IPython Shell.

You'll see that ``` sorted() ``` takes three arguments: ``` iterable ```, ``` key ```, and ``` reverse. ```

``` key=None ``` means that if you don't specify the ``` key ``` argument, it will be ``` None.``` ```reverse=False ``` means that if you don't specify the ``` reverse ``` argument, it will be ``` False ```, by default.

In this exercise, you'll only have to specify ``` iterable ``` and ``` reverse ```, not ``` key ```. The first input you pass to ``` sorted() ``` will be matched to the ``` iterable ``` argument, but what about the second input? To tell Python you want to specify ``` reverse ``` without changing anything about ``` key ```, you can use ``` = ``` to assign it a new value:

```
sorted(____, reverse=____)

```

**Note**: For now, we can understand an ***iterable*** as being any collection of objects, e.g., a List.

Two lists have been created for you. Can you paste them together and sort them in descending order?

```
first = [11.25, 18.0, 20.0]
second = [10.75, 9.50]

```
Use ``` + ``` to merge the contents of ``` first ``` and ``` second ``` into a new list: ``` full ```.

```
full = first + second

```

Call ``` sorted() ``` on ``` full ``` and specify the ``` reverse ``` argument to be ``` True ```. Save the sorted list as ``` full_sorted ```.

```
full_sorted = sorted(full, reverse=True)

```
Finish off by printing out ``` full_sorted ```.

```
print(full_sorted)

```



