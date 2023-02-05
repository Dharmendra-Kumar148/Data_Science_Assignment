# Data_Science_Assignment
PW Skills Assignment Of Data Science

ASSIGNMENT   Date-03/02/2023.

Q1. Which keyword is used to create a function? Create a function to return a list of odd numbers in the range of 1 to 25.

ANS: 'def' keyword is used to create a function.
      
      ## function for return a list of odd numbers.
      
      def oddNumber():                  ''' defition of function '''
          n = []                     
          for i in range(0,50):
              if i % 2 != 0:
                 n.append(i)
          return n       
          
      oddNumber()                       ''' calling function '''
      
  
Q2. Why *args and **kwargs is used in some functions? Create a function each for *args and **kwargs to demonstrate their use.

ANS: *args is used in place of passing "definte and indefinte arguments" OR in other words where numbers of arguments are not knows and **kwargs is used in place of        passing arguments as "key and values" OR in other words passing arguments as "Dictonary" in function.

     ## function for demonstrate *args.
     
     def simple_args(*args):                   ''' definition of function '''
         return n
         
     
     simple_args(1,2,3,4,5,6)                  ''' calling function with more than one argument '''
     simple_args(1,2,3,4,"abhay","yadav")      ''' calling function with different types of arguments '''
     
     
     ## function for demonstrate **kwargs.
     
     def keyValue(**kwargs):                                      ''' definition of function '''       
          return kwargs
          
      
     keyValue(a=12,b=32,c=90,d=[5,6,7,8],e=("Abhay","yadav"))      '''calling function '''
     
     
     
Q3. What is an iterator in python? Name the method used to initialise the iterator object and the method used for iteration.

ANS: iterator is variable which iterates whole loop for a particular task OR in other words 'i' iterates 'for loop' for a given condition than i knowna as iterator.
     OR in other words iterator in python is an object used to iterate over iterable object like list,tuples,dicts,and sets.
     The iterator object is initialized using tier() method.
     It uses next() for iteration.




Q4. What is a generator function in python? Why yield keyword is used? Give an example of a generator function.

ANS: Generator function in python is a like a simple function but in generator function we fetch the data by 'yield' keyword in place of print().
     yield keyword is used to fetch the data on every iteration OR in other words yield is responsible for saving memory because its fetch data instead of storing        the data.
     
     ## example of a generator function  for fibonacci Series.
     
     def fib(n):                  ''' function definition '''
         a,b=0,1
         for i in range(n):
             yield a
             a,b=b,a+b
             
             
     for i in fib(10):             ''' calling function '''
         print(i)
     
     
Q5. Create a generator function for prime numbers less than 1000. 1000. Use the next() method to print the first 20 prime numbers.

ANS: ### prime number using generator function without using next().
     
     def prime(n):                       ''' generator function definition '''
         for i in range(n):
             if i==1 or i==2:
                 yield i
             else:
                 if i % 2 != 0:
                     yield i
       
     
     for i in prime(1000):               ''' generator function calling '''
            print(i)
