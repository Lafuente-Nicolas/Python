# Jour 1
`print` = imprimer

## Define variables of different data types

```python
integer_var = 10 # entier
float_var = 3.14 # décimal
string_var = "AI" # String (chaine de caractères)
list_var = [1, 2, 3] # liste
tuple_var = (4, 5, 6) # tableau
dict_var = {"name": "Alice", "role": "Engineer"} # dictionnaire
bool_var = True # booléen
```

## Print and manipulate variables

```python
print("Integer: ", integer_var) # print 10
print("Float: ", float_var) # print 3.14
print("String: ", string_var + " Bootcamp")
list_var.append(4)
print("List: ", list_var)
print("Tupple: ", tuple_var)
print("Dictionary Value:", dict_var["role"])
print("Boolean: ", bool_var)
```
# jour 2

## Example 1: Checking a condition
```python
 num = -50
 if num > 0:
    print("Positive Number")
 elif num == 0: # elif (else if en js)
     print("Zero")
 else:
     print("Negative Number")
```
## Example 2: Nested conditions (conditions imbriquées)
```python
 age = 3
 if age > 18:
    if age < 30: # 2 if car 2 conditions
       print("Young Adult")
    else:
        print("Adult")
```
## Loops (boucle)

### Loop through a list
```python
fruits = ["apple", "banana", "cherry"]
 for leNomdeLavariable in fruits:
     print(fruit)
```

### Loop with range
```python
 for i in range(5): #va parcourir la liste[0,1,2,3,4]
     print(i)
```


 ### Count down from 5 (compte a rebours)
```python
 count = 5
 while count > 0:
     print(count)
    count -= 1

    print("Outside For Loop")
```
### for i in range(10):

   if i % 2 == 0:
       continue
     print(i)


### for i in range(10):
```python
     if i == 5:
         break # la boucle s'arrete a 5 avec break 
     print(i)
```
### print("Outside For Loop")

```python
 Count down from 5
 count = 5
 while count > 0:
     print(count)
    count -= 1
```
### Exercice 1 : Check if a Number is prime (nombre premier)

```python
num = int(input("Enter a number: ")) # int = nombre premier

if num > 1:
    for i in range(2, int(num**0.5) + 1): # voir en dessous
        if num % i == 0:
            print(f"{num} is not a prime number")
            break
    else:
        print(f"{num} is a prime number")
else:
    print(f"{num} is not a prime number")
```
`in range` est utilisé pour vérifier si une valeur spécifique se trouve dans la séquence générée par la fonction range

### Exercice 2 : Create a Menu-Driven Calculator
```python
def add(a, b): # def = fonction et add = additionner 
    return a + b

def subtract(a, b): # subtract = soustraction
    return a - b

def multiply(a, b): # multiplier
    return a * b

def divide(a, b): # diviser
    if b != 0: # non divisible par 0
        return a / b
    else:
        return "Division by zero is not allowed"
    
while True:
    print("\nMenu:") # \n = ajoute la ligne suivante ou une invite de commande
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exit")
    
    choice = input("Enter your choice: ")
    
    if choice == "5":
        print("Exiting Program.")
        break
    
    num1 = float(input("Enter first number: ")) # float = décimal
    num2 = float(input("Enter second number: "))
    
    if choice == "1": # 1 = addition (regarde au dessus)
        print("Result: ", add(num1, num2)) #additionne num1 et num2
    elif choice == "2":
        print("Result: ", subtract(num1, num2))
    elif choice == "3":
        print("Result: ", multiply(num1, num2))
    elif choice == "4":
        print("Result: ", divide(num1, num2))
    else:
        print("Invclid choice. Please try again.") # imaginons il appuit sur 9, il y a rien
```
# Jour 3

## Fonctions

__fonction = def__
```python 
def function_name(parameters):
     #Code block
   return result
```
## Modules 
```python
import math as m  # m = alias (l'utiliser quand il y a des longs modules)
print(m.sqrt(16)) # sqrt = racine carré
```
### exercice 1 : Create a Function to calculate factorials

`exemple factorial = 5 alors 5*4*3*2*1 = 120`

```python
def factorial(n):
    if n == 0 or n == 1: 
        return 1
    else:
        return n * factorial(n - 1)

def print_factorial(n): 
    result = factorial(n)
    print(f"The factorial of {n} is {result}")
    
print_factorial(5) # factorial de 5 = 120
```
### exemple maths opérations and import
Imaginons que le fichiers se nomme math_operations

```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b != 0:
        return a / b
    else:
        return "Division by zero is not allowed"
```
et la qu'on veut appeler ce fichier pour les fonctions 

```python 
import math_operations as mo # mo = on fait un alias comme le nom est long

num1 = 10
num2 = 5

print("Addition: ", mo.add(num1, num2))
print("Subtraction: ", mo.subtract(num1, num2))
print("Multiplication: ", mo.multiply(num1, num2))
print("Division: ", mo.divide(num1, num2))
```
# Jour 4

## Lists
```python
 Lenom = [1,2,3,4]
print(Lenom[2]) # ça s'arrete a 3 car le 1 est l'index donc 0, le 2 = 1...
print(Lenom[-1]) # cela va donner le dernier chiffre donc 4 , -2 = 3...


Lenom.append("orange") # ajoute "orange" à la liste
Lenom.insert(1, "grape") # ajoute "grape" et devient l'index 1

Lenom.remove("4") # supprime le numéro 4
Lenom.pop() #enlève le dernier élément de la liste

sliced_Lenom = Lenom[1:3] # prend l'index 1 (2) et 2 (3)
```
## Tubles