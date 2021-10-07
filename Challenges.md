# Dart Apprentice

## Chapter 2: Expressions, Variables & Constants

> Challenge 1: Variables
> 
> Declare a constant int called myAge and set it
equal to your age. Also declare an int variable
called dogs and set that equal to the number of
dogs you own. Then imagine you bought a new
puppy and increment the dogs variable by one.

````dart 
void main() {
  int myAge = 19;
  int dogs = 2;
  dogs+=1;
  print(dogs);
}
````
![Challenge 1](/image_2021-10-07_151559.png)
___
> Challenge 2: Make it compile
> 
> Given the following code:

````dart
age = 16;
print(age);
age = 30;
print(age);
````
> Modify the first line so that the code compiles.
Did you use var, int, final or const?

````dart
void main(){
int age = 16;
print(age);  
age = 30;
print(age);
}
````
![Challenge 2](/image_2021-10-07_152554.png)
___
> Challenge 3: Compute the answer
> 
> Consider the following code:

````dart
const x = 46;
const y = 10;
````
> Work out what each answer equals when you add
the following lines of code to the code above:
````dart
const answer1 = (x * 100) + y;
const answer2 = (x * 100) + (y * 100);
const answer3 = (x * 100) + (y / 10);
````
answer1 = 4610

answer2 = 5600

answer3 = 4601

![Challenge 3](/image_2021-10-07_153154.png)
___
> Challenge 4: Average rating
> 
> Declare three constants called rating1, rating2
and rating3 of type double and assign each a
value. Calculate the average of the three and
store the result in a constant named
averageRating.

````dart
void main(){
 double rating1 = 4.5;
 double rating2 = 4;
 double rating3 = 4.7;
 double averageRating = (rating1+rating2+rating3)/3;
 print(averageRating);
}
````
![Challenge 4 ](/image_2021-10-07_153728.png)
___
>Challenge 5: Quadratic equations
>
>A quadratic equation is something of the form
a⋅x² + b⋅x + c = 0.
The values of x which satisfy this can be solved
by using the equation
x = (-b ± sqrt(b² - 4⋅a⋅c)) / (2⋅a).
Declare three constants named a, b and c of type
double. Then calculate the two values for x using
the equation above (noting that the ± means plus
or minus, so one value of x for each). Store the
results in constants called root1 and root2 of
type double. 


````dart
import 'dart:math';
void main(){
  double a = 4;
  double b = 16;
  double c = 16;
  double root1 =(-b + sqrt(b*b - 4*a*c)) / (2*a);
  double root2 =(-b - sqrt(b*b - 4*a*c)) / (2*a);
  print(root1);
  print(root2);
}
````
![Challenge 5](/image_2021-10-07_154253.png)

___

## Chapter 3: Types & Operations

> Challenge 1: Teacher’s grading
> 
>You’re a teacher, and in your class, attendance is
worth 20% of the grade, the homework is worth
30% and the exam is worth 50%. Your student
got 90 points for her attendance, 80 points for
her homework and 94 points on her exam.
Calculate her grade as an integer percentage
rounded down. 

````dart
void main(){
 double homewrk=80;
 double attendance= 90;
 double xam=94;
 double hwkMark = (30/100)*homewrk;
 double attendMark  = (20/100)* attendance;
 double xamMark = (50/100)*xam;
  print((hwkMark + attendMark + xamMark).round());
}
````
![Challenge 1](/image_2021-10-07_155948.png)
___
>Challenge 2: Same same, but different
>
>This string has two flags that look the same. But
they aren’t! One of them is the flag of Chad and
the other is the flag of Romania.

````dart
const twoCountries = '🇹🇩🇷🇴';
````
> Which is which?

___
>Challenge 3: How many?
>
>Given the following string:
````dart
const vote = 'Thumbs up! 
````
>How many UTF-16 code units are there?

10
>How many Unicode code points are there?

10
>How many Unicode grapheme clusters are there?

````dart
import 'package:characters/characters.dart';
void main() {
const vote = 'Thumbs up! 👍🏿';
print(vote.codeUnits.length);
print(vote.runes.length);
print(vote.characters.length);
}
````
___
>Challenge 4: Find the error
>
>What is wrong with the following code?
````dart
const name = 'Ray';
name += ' Wenderlich';
````
Since name has been declared by const type, We couldn't make changes further. 

__Constant variables can't be assigned a value.__
___
> Challenge 5:What type? 
> 
> What’s the type of value?

````dart
const value = 10 / 2;
````
Type - __double__ 
___
> Challenge 6: In summary
> 
> What is the value of the constant named summary?
````dart
const number = 10;
const multiplier = 5;
final summary = '$number \u00D7 $multiplier
= ${number * multiplier}';
````
10 x 5 = 50

![Challege 6](/image_2021-10-07_162019.png)
___
## Chapter 4: Control Flow
