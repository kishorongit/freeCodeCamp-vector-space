# freeCodeCamp-vector-space

Learn special methods by building a vector space.

## Introduction to Special Methods

A variety of instance methods are reserved by Python which affects the behavior of a class, especially an object's high level behavior and its interactions with operators. These are are known as special methods. The names of these methods follow a specific naming pattern that include both a leading and trailing double underscore in their names as `__<name>__`. `__init__` and `__str__` are examples of special methods. Accordingly, they can also be referred to as magic methods or "dunder" (double underscore) methods. Thery are called in specific situations such as `__init__` during instantiation and `__str__` when the object is printed or passed to `str()`.

## List of special methods covered

| Special Method     | Description                                                                                |
| ------------------ | ------------------------------------------------------------------------------------------ |
| `__init__`         | Initialize new instance                                                                    |
| `__str__`          | Printable (human-readable) string representation                                           |
| `__dict__`         | Object's (writable) attributes dictionary                                                  |
| `__repr__`         | “official” string representation needed to instantiate an object                           |
| `__class__`        | Instance's class                                                                           |
| `__name__`         | Name of the class, fucntion, method, descriptor, or generator isntance                     |
| `__getattribute__` | Instance's attribute. If not found serach at class level, and eventually in parent classes |
| `__getattr__`      | Fallback when the usual attribute accessing procedure fails                                |
| `__add__`          | Addition of two objects using `+` operator                                                 |
| `__sub__`          | Subtraction of two objects using `-` operator                                              |
| `__mul__`          | Multiplication of two objects using `*` operator                                           |
| `__eq__`           | Comparision of two objects using `==` operator                                             |
| `__ne__`           | Comparision of two objects using `!=` operator                                             |
| `__lt__`           | Comparision of two objects using `<` operator                                              |
| `__le__`           | Comparision of two objects using `<=` operator                                             |
| `__ge__`           | Comparision of two objects using `>=` operator                                             |

For available special method names refer [Python Data model][1].

## Additional Concepts

### 1. Keyword-only arguments

According to [PEP 3102][2], "keyword-only" arguments are function arguments that can only be supplied by keyword and which will never be automatically filled in by a positional argument. For further readings, refer [here][3].

### 2. Built-in functions

-   `vars()` - Returns the `__dict__` attribute of that object
-   `getattr()` - Returns the value of the named attribute of object

### 3. Spcial value

-   `NotImplemented` - A special value used to indicate that an operation is not implemented for a specific case. It does not raise an exception immediately. Instead, it signals to ask to the other operand how to perform the operation. If the request cannot be satisfied, a `TypeError` is returned by default.

<!-- List of references -->

[1]: https://docs.python.org/3/reference/datamodel.html#special-method-names
[2]: https://peps.python.org/pep-3102/
[3]: https://realpython.com/python-asterisk-and-slash-special-parameters/
