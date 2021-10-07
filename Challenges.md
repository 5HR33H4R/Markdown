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



