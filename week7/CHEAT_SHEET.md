# Python Cheat Sheet

## Types

* Strings - any kind of characters in quotes
  * `"This is 1 single string, it's in quotes."`
* Integer - numbers, no quotes
  * `1`
* Boolean
  * `True` or `False`
* Lists - collection of items, in `[]` brackets

```python
["String", 1, 2, "Another string"]
````

* Dictionary - collection of items using `key:value` pairs

```python
{
    "name": "Bruce Wayne",
    "profession": "Batman"
}
 ```

## Loops

A `for` loop will loop over each item in a collection of items.

```python
list_of_numbers = [1,2,3]

for number in list_of_numbers:
    # For this example, we'll print each number
    print(number)
```

A `while` loop will loop over items until a condition is no longer `True`

```python
my_string = "Green Lantern Corp"
index = 0

while index < len(my_string):
    # For this example, we'll print each character in the string based on the value of the index
    print(my_string[index])
```

## Functions

A function will have **four** key parts:

1. The function keyword
2. A unique name (make it descriptive!)
3. Parentheses, `()`, follow the name and can accept parameters (if needed!)
4. The function body, which will `return` a value
    * **REMINDER**: If no value is _explicitly_ returned, Python will return `None`

```python
# name is a parameter, we'll pass the value as an argument when we call the function
def greeting(name):
    return "Hello %s!" % (name)

# The variable `sean` will be assigned the value returned from the `greeting()` function
# We pass the string "Sean" as an argument into the function `greeting()`
sean = greeting("Sean")

print(sean)
```
