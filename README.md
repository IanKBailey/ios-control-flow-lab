# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```

- A
- B
- C
- D

```
a,c,d
```
***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```

- appInfo.0 hasn't released yet
- myCoolApp hasn't released yet
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error
```
myCoolApp hasn't released yet
```
***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```

- A
- B
- C
- D
```
D
```

***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}
```

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- No default case in the switch statement
- No print statement right outside the switch statement
````
c

`````
***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below
```
```
let currentWeather = "rain"
switch currentWeather {
case "rain":
    print("bring a raincoat")
case "sunny":
    print("it's a nice day")
case "snowy":
    print("bring a coat")
default:
    print("have a nice day")
}
```

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below
```
```
let fullname = "\(firstName)" + " " + "\(lastName)"
print(fullname)
```

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift
if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

//Re-written statement here

```
```

 var temperatureInFahrenheit = 40

switch temperatureInFahrenheit {
case  1..<40:
    print("it's really cold")
case 85..<120:
    print("it's really hot")
default:
    print("the weather is moderate")
}
```
***

## Question 8

Complete the following code so that "You win!" is printed.

```swift
if {
 print("You win!")
} 
else {
 print("You lose!")
}
```

```

var points = 100

if points >= 50{
 print("You win!")
}
else {
 print("You lose!")
}


```
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
Example 1:

Input:
var numberOfSides = 4

Output:
Square

Example 2:

Input:
var numberOfSides = 2

Output:
Error

```
```
var numberOfSides = 3

switch numberOfSides {
case 3:
    print("triangle")
case 4:
    print("square")
case 5:
    print("pentagon")
case 6:
    print("hexagon")
case 7:
    print("heptagon")
case 8:
    print("octagon")
case 9:
    print("nonagon")
case 10:
    print("decagon")
default:
    print("out of range")
}

```
***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
Numeric Score 	Letter Grade
100 	A+
90 - 99	A
80 - 89	B
70 - 79 	C
65 - 69 	D
Below 65 	F
```

```
var grade = 89

switch grade {
case 100 :
    print("A+")
case 90...99:
    print("A")
case 80...89:
    print("B")
case 70...79:
    print("C")
case 65...69:
    print("D")
default:
    print("F")
}
```
***

## Question 11

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
let firstName = "Peter"

if firstName == "Peter" {
 let lastName = "Gabriel"
} else if firstName == "Phil" {
 let lastName = "Collins"
}
let fullName = firstName + " " + lastName
```

```

var firstName = "Peter"
var lastName = " "
var fullName = " "
if firstName == "Peter" {
    lastName = "Gabriel"
    fullName = firstName + " " + lastName
    print(fullName)
} else if firstName == "Phil" {
    lastName = "Collins"
    fullName = firstName + " " + lastName
    print(fullName)
}
```
***

## Question 12

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

```swift
let nameAndBirthYear: (String, Int)
```
***
```
let nameAndBirthYear = (String:"Hello", Int:30)
if nameAndBirthYear.Int >= 20 && nameAndBirthYear.Int < 30{
    print("you are in your twenties")
} else {
    print("I don't know what decade of life you're in!")
}

switch nameAndBirthYear.Int {
case 20...29 :
    print("You are in your twenties")
default:
    print("I don't know what decade of life you're in!")
    
}
```

## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
```
What happens when you change number to:

-a. 365?

-b. 1024?

-c. 65?

What happens when you remove the default clause?

***
```
A. it will say: "Days in year"
B. it will say: "Bytes in kilobytes"
C. it will run the default
D. if you remove the default clause it wouldn't compile

```

## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
}
```

```
A.
if population > 10000 {
 message = "\(population) is a large town"
    print(message)
} else if population <= 10000 && population >= 5000 {
    print("It's a medium size town")
}

B. if population > 10000 {
 message = "\(population) is a large town"
    print(message)
} else if population <= 10000 && population >= 5000 {
   message = ("It's a medium size town")
    print(message)
    
} else {
message = ("It's a med-size town")
    print(message)
}

C.
if population > 10000 {
 message = "\(population) is a large town"
    print(message)
} else if population <= 10000 && population >= 5000 {
   message = ("It's a medium size town")
    print(message)
    
}
switch population {
case 5000...10000:
    print("it's a medium sized town")
default:
    print("it's a large sized town")
}



```
***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

b. Using a switch statement

```swift
let myTuple: (Int, Int) = (5, 10)
```

```
if myTuple.0 + myTuple.1 >= 15 {
    print("the value is 15 or more")
}

```
***
```
let myTuple: (Int, Int) = (5, 10)

if myTuple.0 + myTuple.1 >= 15 {
    print("the value is 15 or more")
}

switch myTuple.0 + myTuple.1 >= 15 {
case true :
    print("It's greater then 15")
default:
    print("less then 15")
}
```
