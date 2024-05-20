### Question1 : Why do you use with in python ?

Solution: In Python, the with statement is used to wrap the execution of a block of code within methods . The primary benefit of using the with statement is that it ensures that resources are properly and automatically cleaned up after their use, even if errors occur during the execution of the block.

### Question2: What is tell() method in python?

Solution: The tell() method in Python is used with file objects to get the current position of the file pointer within the file.

### Question3: What is an API?

Solution: An API (Application Programming Interface) is a set of rules and protocols that allows different software applications to communicate with each other. It defines the methods and data structures that applications use to request and exchange information. APIs enable developers to access the functionality of another application, service, or platform without having to understand its internal implementation.

### Question4: Difference between setTimeout and set interval in js?

Solution: 
- setTimeout: Executes the function only once after the specified delay.
- setInterval: Executes the function repeatedly at the specified interval until it is stopped.  It continues to execute until explicitly stopped using clearInterval(intervalID).

### Question5: What are SSH key?

Solution: SSH (Secure Shell) keys are cryptographic keys used for authenticating and securing communication between an SSH client and an SSH server. SSH keys are part of public-key cryptography, which involves a pair of keys: a private key and a public key. These keys are used to create a secure, encrypted connection over an unsecured network.

### Question6 : How to convert array into object in js?

Solution: 

- Method 1: Using Object.assign
  ```javascript
    const array = ['a', 'b', 'c'];
    const obj = Object.assign({}, array);
    console.log(obj);
    // Output: { 0: 'a', 1: 'b', 2: 'c' }

  ```
- Method 2: : Manually Creating an Object
  ```javascript
    const array = ['a', 'b', 'c'];
    const obj = {};
    array.forEach((value, index) => {
        obj[index] = value;
    });
    console.log(obj);
    // Output: { 0: 'a', 1: 'b', 2: 'c' }

  ```

### Question7 : What data types does JavaScript support?

Solution: JavaScript supports a variety of data types, which can be broadly categorized into primitive types and object types.

1. **Primitive Data Types :**
   - String
   - Number
   - BigInt
   - Boolean
   - Undefined 
   - Null
   - Symbol
2. **Object Types :**
   - Object
   - Array
   - Function
   - Date
   - RegExp
   - Map
   - Set

### Question8 : How would you find the most common elements in a list in python?

Solution: 
- Method1 : Using a dictionary
  ```python
    # Example list
    elements = ['a', 'b', 'c', 'a', 'b', 'a']

    # Count the elements using a dictionary
    count_dict = {}
    for element in elements:
      if element in count_dict:
          count_dict[element] += 1
      else:
          count_dict[element] = 1

    # Sort the dictionary by values (counts) in descending order
      sorted_elements = sorted(count_dict.items(), key=lambda     item: item[1], reverse=True)
      print(sorted_elements)

    # If you want just the top N most common elements
    top_n = 2
    most_common_top_n = sorted_elements[:top_n]
    print(most_common_top_n)

  ```

- Method2 : Using collections.Counter
  ```python
    from collections import Counter

    # Example list
    elements = ['a', 'b', 'c', 'a', 'b', 'a']

    # Count the elements
    counter = Counter(elements)

    # Find the most common elements
    most_common_elements = counter.most_common()  # This returns a list of tuples (element, count)
    print(most_common_elements)

    # If you want just the top N most common elements, specify N
    top_n = 2
    most_common_top_n = counter.most_common(top_n)
    print(most_common_top_n)

  ```


### Question9: What is currying in js?

Solution: Currying in JavaScript is a technique of transforming a function that takes multiple arguments into a series of functions that each take a single argument. This is achieved by creating a function that returns another function, which continues to accept arguments until all arguments have been provided. Once all arguments are provided, the final function executes the original multi-argument function.

```javascript
  function curriedAdd(x) {
    return function(y) {
      return function(z) {
        return x + y + z;
      }
    }
  }

  // Usage
  const addFive = curriedAdd(2)(3); // returns a function
  const result = addFive(4);        // returns 9
  console.log(result);              // 9

  // Or, all at once
  const resultAllAtOnce = curriedAdd(2)(3)(4);
  console.log(resultAllAtOnce);     // 9

```

### Question10 : How do we define random function in python and what is the use of it ?

Solution: In Python, the random module provides a variety of functions to generate random numbers, select random elements, and perform random permutations.

```python
  import random
  random_int = random.randint(1, 10)
  print(random_int)  # Output: a random integer between 1 and 10, inclusive

```

Uses:
- Games: Generating random events, random shuffles, or random positions.
- Data Analysis: Randomly splitting datasets into training and testing sets.
  
### Queston11 : How do you change the permissions of a file?

Solution: The chmod command allows you to modify the file permissions for the owner, group, and others.

```bash
  chmod 755 filename
```

If many files are there in a file, then if we want to change the permission of each file:

```bash
  chmod -R 755 filename
```
