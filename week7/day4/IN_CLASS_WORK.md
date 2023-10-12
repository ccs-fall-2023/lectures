# In Class Work

Pun not necessarily intended...

## Working with an existing class

Given the following `Person` class:

```python
class Person:
    def __init__(self, name, email, phone):
      self.name = name
      self.email = email
      self.phone = phone

    def greet(self, other_person):
      print('Hello %s, I am %s!' % (other_person.name, self.name))
```

Write code to:

* Instantiate an instance object of Person with name of 'Sonny', email of 'sonny@hotmail.com', and phone of '483-485-4948', store it in the variable `sonny`.
* Instantiate another person with the name of 'Jordan', email of 'jordan@aol.com', and phone of '495-586-3456', store it in the variable `jordan`.
* Have `sonny` greet `jordan` using the greet method.
* Have `jordan` greet `sonny` using the greet method.
* Write a print statement to print the contact info (email and phone) of Sonny.
* Write another print statement to print the contact info of Jordan.

---

### Make your own class

Create a class `Vehicle`. A `Vehicle` object will have 3 attributes:

* make
* model
* year

A vehicle is created like this:

`car = Vehicle('Nissan', 'Leaf', 2015)`

And you can access it's attributes individually like so:

```python
print(car.make, car.model, car.year)
```

#### Add a method

Add a `print_info` method to the `Vehicle` class. It will print out the vehicle's information like so:

```python
car.print_info()
```

Will output:

```python
2015 Nissan Leaf
```

---

## Expanding classes

### Add another method

Go back to the `Person` class.

```python
class Person:
    def __init__(self, name, email, phone):
         self.name = name
         self.email = email
         self.phone = phone

     def greet(self, other_person):
         print('Hello %s, I am %s!' % (other_person.name, self.name))
```

#### Add a Method

Add a `print_contact_info` method to the `Person` class that will print out the contact info for a object instance of Person.

```python
sonny.print_contact_info()
```

Should generate this output:

```bash
Sonny's email: sonny@hotmail.com
Sonny's phone number: 483-485-4948
```

#### Add an instance variable (attribute)

Add a `friends` instance variable (attribute) to the `Person` class.

You will initialize it to an empty list within the constructor `__init__`.

Once you've done this you should be able to add a friend to a person using list's append method:

`jordan.friends.append(sonny)`
`sonny.friends.append(jordan)`

You should also be able to get the number of friends a person has by using the len function on his friends:

```python
len(jordan.friends)
```

Will return:

```python
1
```

#### Add an `add_friend` method

The fact that a person's friends attribute is a list is an implementation detail of the `Person` class.

Occassionally you'll want to hide implementation details from the users of your object/class. Implement an `add_friend` method to `Person`, so that in order to add a friend you call this method:

`jordan.add_friend(sonny)`

instead of:

`jordan.friends.append(sonny)`

#### Add a `num_friends` method

We also want to hide the implementation detail that there is a friends attribute containing a list of friends.

To do this, we'll implement a `num_friends` method which returns the number of friends for a person.

For example:

```python
jordan.num_friends()
1
```

#### Count number of greetings

We want to count the number of times a person has greeted someone. To do this, we'll add another attribute, `greeting_count`, and initialize it to `0`. Then each time the greet method is called, we'll increment `greeting_count` by `1`.

The output will resemble the following:

```bash
>>> sonny.greeting_count
0
>>> sonny.greet(jordan)
>>> sonny.greeting_count
1
>>> sonny.greet(jordan)
>>> sonny.greeting_count
2
```

### Working with `__str__`

You may notice that when you are working with a person object, it's representation in the Python shell is pretty cryptic and unhelpful:

```bash
>>> print(jordan)
<__main__.Person object at 0x106976410>
```

Adding the `__str__` method to the `Person` class and have it return a string. Whatever you return there will be used to "represent" your person object.

For example, say I want a `Person` to be represented like this:
Jordan jordan@aol.com 495-586-3456

I could implement __str__ like this:

```python
def __str__(self):
     return 'Person: {} {} {}'.format(self.name, self.email, self.phone)
```

Implement your own `__str__` method, and you can represent your person objects however you want. Incidentally, `__str__` is also used when you use convert your object to a string: i.e. `str(jordan)`.

---

### Bonus Challenge

Keep track of the number of unique people a person has greeted, and be able to report that number via a `num_unique_people_greeted method`:

```bash
>>> sonny.num_unique_people_greeted()
0
>>> sonny.greet(jordan)
>>> sonny.num_unique_people_greeted()
1
>>> sonny.greet(jordan)
>>> sonny.num_unique_people_greeted()
1
>>> sonny.greet(dee_ann)
>>> sonny.num_unique_people_greeted()
2
```
