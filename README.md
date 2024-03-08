# R-Tutorial

R language was developed by statisticians for statisticians. This means R should be a goto language for any kind of statistical analysis.

## Installing R

To install R, go to https://cloud.r-project.org/ and download the latest version of R for Windows, Mac or Linux.
On opening the site, you will be able to view the following page:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/6f73f9b5-5a6f-406d-af19-46cd9935db19)

On clicking `Download R for Windows`, you have to click on "install R for the first time":

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/65a580a0-c192-4a2e-8479-668181143565)

Then on clicking,,downloading will start:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/c76997db-10e7-4c21-aa08-18fe20b86aa3)

When you have downloaded and installed R, you can run R on your computer.
<br><br>
## Installing R Studio

After installing R, we need an IDE(Integrated Development Environment) called RStudio.
To install R studio, go to https://posit.co/download/rstudio-desktop/
Scroll down to find your system version:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/e766a435-61ed-4148-8f61-c7ba2b7ad713)
<br><br>
## Variables in R

Variables are temporary storage spaces.

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/9f9d0a49-3a48-449a-aac9-e74b7423f002)

Variables are containers for storing data values.

R does not have a command for declaring a variable. A variable is created the moment you first assign a value to it. To assign a value to a variable, use the `<-` sign. To output (or print) the variable value, just type the variable name:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/3615fcd8-c961-4ac0-91b3-3d43e2cb7a6c)

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/fe4db6d2-0136-4ff3-9e7a-10c2cb16a276)

In other programming language, it is common to use `=` as an assignment operator. In R, we can use both `=` and `<-` as assignment operators.
However, `<-` is preferred in most cases because the `=` operator can be forbidden in some context in R.

`NOTE:` In R, you can print a variable by simply typing its name. However, R does have a print() function available if you want to use it. This might be useful if you are familiar with other programming languages, such as Python, which often use a print() function to output variables.
And there are times you must use the print() function to output code, for example when working with for loops(we will discuss later).
<br><br>
## Datatypes in R

Whenever you create a variable, you store some data in it. The type of that data is called datatype.

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/72ba7061-9121-47cb-882c-092b9a3c5790)

Variables can store data of different types, and different types can do different things.
In R, variables do not need to be declared with any particular type, and can even change type after they have been set, this shows R is a **dynamically typed** language:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/16208ffd-8632-4493-b11c-f10717a1f046)

<br>
Basic data types in R can be divided into the following types:

   - numeric - (10.5, 55, 787)
   - integer - (1L, 55L, 100L, where the letter "L" declares this as an integer)
   - complex - (9 + 3i, where "i" is the imaginary part)
   - character (a.k.a. string) - ("k", "R is exciting", "FALSE", "11.5")
   - logical (a.k.a. boolean) - (TRUE or FALSE)

We can use the class() function to check the data type of a variable:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/befdf71a-dd8d-4106-8bd2-65754ce26daa)

`NOTE:` You can clear the console by `Ctrl+L`. You can also goto the previous typed commands by `Up` arrow.
<br><br>
## Operators in R

Operators are used to perform operations on variables and values.

In the example below, we use the + operator to add together two values:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/28dcf6d4-f23c-4f2e-a5b6-8f2082fabf30)

R has following types of operators:

- Arithmetic operators

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/f3df5826-e819-4eb7-9054-8c6c4e1d7579)

- Assignment operators

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/01a44bd7-1dd8-49b0-b263-6bd4c8763dda)

`Note:` <<- is a global assigner. We will learn more about this later. It is also possible to turn the direction of the assignment operator. x <- 3 is equal to 3 -> x

- Comparison operators

  ![image](https://github.com/Diya050/R-Tutorial/assets/124448340/e02936fc-7380-48e6-8173-bc14ef973d9c)

- Logical operators

  ![image](https://github.com/Diya050/R-Tutorial/assets/124448340/19708bf8-7dcc-4c73-b204-e8a81a3f9289)

- Miscellaneous operators

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/d799a710-c0c7-47cd-a651-c967e208bb25)
<br><br>

## Data Structures in R

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/02430e15-c2b3-457f-a43a-ec3f91a5fca2)

<br><br>

### R VECTORS

A vector is simply a list of items that are of the same type.

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/64ce0e23-5015-4102-b845-b4aa4e1e0e94)

To combine the list of items to a vector, use the c() function and separate the items by a comma.

In the example below, we create a vector variable called fruits, that combine strings:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/5e984c95-273f-43df-9cbd-44fa62ee737e)

To create a vector with numerical values in a sequence, use the : operator:

```R
> numbers <- 1:10
> 
> numbers
 [1]  1  2  3  4  5  6  7  8  9 10
> 
```

You can also create numerical values with decimals in a sequence, but note that if the last element does not belong to the sequence, it is not used:

![image](https://github.com/Diya050/R-Tutorial/assets/124448340/1fdcecad-81ad-4f67-bbc3-3e2f575cbab5)

In the example below, we create a vector of logical values:

```R
> # Vector of logical values
> log_values <- c(TRUE, FALSE, TRUE, FALSE)
> 
> log_values
[1]  TRUE FALSE  TRUE FALSE
> 
```

#### **Vector Length:**

To find out how many items a vector has, use the length() function:

```R
> fruits <- c("banana", "apple", "orange")
> 
> length(fruits) 
[1] 3
> 
```

#### **Sort a Vector:**

To sort items in a vector alphabetically or numerically, use the sort() function:

```R
> numbers <- c(13, 3, 5, 7, 20, 2)
> 
> sort(numbers) 
[1]  2  3  5  7 13 20
> numbers
[1] 13  3  5  7 20  2
> 
> sorted_numbers <- sort(numbers)
> sorted_numbers
[1]  2  3  5  7 13 20
> numbers
[1] 13  3  5  7 20  2
>
```

#### **Access Vectors:**

You can access the vector items by referring to its index number inside brackets []. The first item has index 1, the second item has index 2, and so on:

```R
> fruits <- c("banana", "apple", "orange")
> 
> fruits[1] 
[1] "banana"
```
You can also access multiple elements by referring to different index positions with the c() function:

```R
> fruits <- c("banana", "apple", "orange", "mango", "lemon")
> 
> fruits[c(1, 3)] 
[1] "banana" "orange"
>
>
> fruits <- c("banana", "apple", "orange", "mango", "lemon")
> 
> fruits[c(1:3)]
[1] "banana" "apple"  "orange"
>
```

You can also use negative index numbers to access all items except the ones specified:

```R
> fruits <- c("banana", "apple", "orange", "mango", "lemon")
> 
> fruits[c(-1)] 
[1] "apple"  "orange" "mango"  "lemon" 
> 
```

#### **Change an Item:**

To change the value of a specific item, refer to the index number:

```R
> fruits <- c("banana", "apple", "orange", "mango", "lemon")
> 
> fruits[1] <- "pear"
> 
> fruits 
[1] "pear"   "apple"  "orange" "mango"  "lemon" 
> 
```

#### **Repeat Vectors:**

To repeat vectors, use the rep() function:
- Repeat each value:
 
```R
> repeat_each <- rep(c(1,2,3), each = 3)
> 
> repeat_each 
[1] 1 1 1 2 2 2 3 3 3
>
```
- Repeat the sequence of the vector:

```R
> repeat_times <- rep(c(1,2,3), times = 3)
> 
> repeat_times 
[1] 1 2 3 1 2 3 1 2 3
>
```
- Repeat each value independently:

```R
> repeat_indepent <- rep(c(1,2,3), times = c(5,2,1))
> 
> repeat_indepent 
[1] 1 1 1 1 1 2 2 3
> 
```

#### **Generating Sequenced Vectors:**

To make bigger or smaller steps in a sequence, use the seq() function:

```R
> numbers <- seq(from = 0, to = 100, by = 20)
> 
> numbers 
[1]   0  20  40  60  80 100
> 
```

`NOTE:` The `seq()` function has three parameters: `from` is where the sequence starts, `to` is where the sequence stops, and `by` is the interval of the sequence.

### R LISTS

A list in R can contain many different data types inside it. A list is a collection of data which is ordered and changeable.

To create a list, use the list() function:
```R
> thislist <- list("apple", "banana", "cherry")
> 
> thislist 
[[1]]
[1] "apple"

[[2]]
[1] "banana"

[[3]]
[1] "cherry"
>
```

#### Access Lists:

You can access the list items by referring to its index number, inside brackets. The first item has index 1, the second item has index 2, and so on:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> thislist[1] 
[[1]]
[1] "apple"

>
```
#### Change Item Value

To change the value of a specific item, refer to the index number:
```R
> thislist <- list("apple", "banana", "cherry")
> thislist[1] <- "blackcurrant"
> 
> thislist 
[[1]]
[1] "blackcurrant"

[[2]]
[1] "banana"

[[3]]
[1] "cherry"

> 
```

#### List Length:

To find out how many items a list has, use the length() function:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> length(thislist) 
[1] 3
> 
```

#### Check if Item Exists:

To find out if a specified item is present in a list, use the %in% operator:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> "apple" %in% thislist 
[1] TRUE
> 
> "mango" %in% thislist
[1] FALSE
> 
```

#### Add List Items:

To add an item to the end of the list, use the append() function:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> append(thislist, "orange") 
[[1]]
[1] "apple"

[[2]]
[1] "banana"

[[3]]
[1] "cherry"

[[4]]
[1] "orange"

> 
```

To add an item to the right of a specified index, add "after=index number" in the append() function:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> append(thislist, "orange", after = 2) 
[[1]]
[1] "apple"

[[2]]
[1] "banana"

[[3]]
[1] "orange"

[[4]]
[1] "cherry"

>
```

#### Remove List Items:

You can also remove list items. The following example creates a new, updated list without an "apple" item:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> newlist <- thislist[-1]
> 
> newlist 
[[1]]
[1] "banana"

[[2]]
[1] "cherry"

> 
```

#### Range of Indexes

You can specify a range of indexes by specifying where to start and where to end the range, by using the : operator:

```R
> thislist <- list("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
> 
> (thislist)[2:5] 
[[1]]
[1] "banana"

[[2]]
[1] "cherry"

[[3]]
[1] "orange"

[[4]]
[1] "kiwi"

> 
```
`NOTE:` The search will start at `index 2 (included)` and end at `index 5 (included)`. Remember that the first item has index 1.


#### Loop Through a List:

You can loop through the list items by using a for loop:

```R
> thislist <- list("apple", "banana", "cherry")
> 
> for (x in thislist) {
+     print(x)
+ } 
[1] "apple"
[1] "banana"
[1] "cherry"
> 
```

#### Join Two Lists:

There are several ways to join, or concatenate, two or more lists in R.

The most common way is to use the c() function, which combines two elements together:

```R
> list1 <- list("a", "b", "c")
> list2 <- list(1,2,3)
> list3 <- c(list1,list2)
> 
> list3 
[[1]]
[1] "a"

[[2]]
[1] "b"

[[3]]
[1] "c"

[[4]]
[1] 1

[[5]]
[1] 2

[[6]]
[1] 3

> 
```
