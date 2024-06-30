[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15348760&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   
   - Python- One of the most popular programming languages.
   - Features-Free and open source, Community support, standard library, easy to code, easy to read(https://www.geeksforgeeks.org/python-features/).
   - Python is used in data science and data analytics. Numerical computation are done using the library known as Numpy.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   - Search  https://www.python.org/downloads/ on your web browser
   - Select Python version to download
   - Click on Install now
   - Select Customize installation and proceed.
   - Click on the Add Path check box, it will set the Python path automatically on your environmental path
   - Continue until installation is done
   
   - To verify Installation:
      - Open Command prompt
      - Write the command :python --version
      - This should return the version of python installed in your computer system
   
   - To set up virtaul environment
      -  OPEN Command Prompt and write the below commands:
         - mkdir Myproject
         - cd Myproject
         - pip install virtualenvironment


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   -print ("Hello, World!")

      - print()=outputs data to the console
      - ""(closed quotation)- used to represent text

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   - Data types-
      - Text Type:	str- sequence of charecters enclosed in quotation marks
         - "Hello, World!"
      - Numeric Types:	int, float, -Numbers
         - x = 20
      - Sequence Types:	list- ordered collection of items. Closed in parentheses
         - x = ["apple", "banana", "cherry"]
      - Boolean Type:	bool-represent one of the two values
         - x = True
         
5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
      - Conditional statements and loops are essential control structures in Python, enabling decision-making and repetitive actions. 
      - 'If-else' statement
         - a = 3
           if a > 5:
                  print("a is greater than 5")
            else:
                  print("a is not greater than 5")

      - 'for' loop
        - >>> countries =['South Africa', 'Kenya', 'Niger']
          >>> for country in countries:
          ...       print(country)
          ...
          South Africa
          Kenya
          Niger

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

      - Blocks of reusable code designed to perform a specific task. They allow for more organized, readable and reusable code.
      - Example:
         >>> def add(a, b):
         ...     return a + b
         ...
         >>> result = add(5, 3)
         >>> print(result)
         8

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   
       - The difference is that lists allows duplicates in theier data whereas dictionaries do not allow duplicates in their data.
       - dictionary:
       >>> thisdict = {
       ...  "Continent": "Africa",
       ...   "country": "South Africa",
       ...   "Freedom": 1994,
       ...   "Continent":"Africa"
       ... }
       >>> print(thisdict)
       {'Continent': 'Africa', 'country': 'South Africa', 'Freedom': 1994}

       - Lists:
       >>> thislist = {
       ...   "Continent": "Africa",
       ...   "country": "South Africa",
       ...   "Freedom": 1994,
       ...   "Continent":"Africa"
       ... }
       >>> print(thislist)
       {'Continent': 'Africa', 'country': 'South Africa', 'Freedom': 1994}

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
    - Exception Handling- allows you to handle errors and execute code even if an error occurs.
    def read_file(file_path):
    try:
        # Attempt to open the file
        file = open(file_path, 'r')
        
        # Attempt to read the file contents
        content = file.read()
        print("File content:")
        print(content)
        
    except FileNotFoundError:
        # Handle the case where the file does not exist
        print(f"Error: The file '{file_path}' was not found.")
        
    except IOError:
        # Handle other I/O errors (e.g., permission denied)
        print(f"Error: An I/O error occurred while trying to read the file '{file_path}'.")
        
    finally:
        # Ensure that the file is properly closed
        try:
            file.close()
            print("File has been closed.")
        except NameError:
            # Handle the case where the file was never opened
            print("File was never opened, so no need to close it.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
    
    - Modules: Reusable pieces of code, using `import` to include  them.Packages-Collections of modules, using `pip` to install packages.

    - Write the below command on Command prompt to install Numpy 
      - pip install numpy
    - To import your script, write the below command on python
      >>>import numpy as np
      >>> arr= np.array([1,2,3,4,5])
      >>> print(arr)
         [1 2 3 4 5]

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    - Given that the file name is "File", to read the file, you use the below commands:
      f = open("File.txt", "r")
      print(f.read())

   - Writes a list of string:
      def write_list_to_file(C:\Recapproject, string_list):
         try:
            with open(C:\Recapproject, 'w') as file:
               for string in string_list:
                  file.write(string + '\n')
            print(f"Successfully wrote to the file '{file_path}'.")
         except IOError:
            print(f"Error: An I/O error occurred while trying to write to the file '{file_path}'.")
            


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


