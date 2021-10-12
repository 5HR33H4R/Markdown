# Dart answers
## Chapter 2: Expressions,Variables & Constants
> Challenge 1: Variables
Declare a constant int called myAge and set it
equal to your age. Also declare an int variable
called dogs and set that equal to the number of
dogs you own. Then imagine you bought a new
puppy and increment the dogs variable by one.

```dart
void main() {
const int myAge =20;
  int dogs=0;
  dogs +=1;
print ('I own $dogs dog');
 }
 
## 
 >  Challenge 2: Make it compile
Given the following code:
age = 16;
print(age);
age = 30;
print(age);
Modify the first line so that the code compiles.
Did you use var, int, final or const?

```dart 
void main() {
 var age = 16;
print(age);
   age = 30;
print(age);
 }

 
