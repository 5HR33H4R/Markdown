# Dart Apprentice

## Chapter 2: Expressions, Variables & Constants

> Challenge 1: Variables
Declare a constant int called myAge and set it
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

> Challenge 2: Make it compile
Given the following code:
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

> Challenge 3: Compute the answer
Consider the following code:
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

> Challenge 4: Average rating
Declare three constants called rating1, rating2
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

>Challenge 5: Quadratic equations
A quadratic equation is something of the form
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


