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