## What are Pointers?
** A pointer is a variable whose value is the address of another variable. A pointer is a variable that holds a memory address. **

## addressing
When a variable is created in C++, a memory address is assigned to the variable. And when we assign a value to the variable, it is stored in this memory address.

## What is polymorphism and example?

A person at the same time can have different characteristics. Like a man at the same time is a father, a husband, an employee. So the same person posses different behavior in different situations. This is called polymorphism.

## What is abstraction and example?

In simple terms, abstraction “displays” only the relevant attributes of objects and “hides” the unnecessary details.

## Recursion
Recursion is a method in C++ which calls itself directly or indirectly until a suitable condition is met.

Ex:
#include<iostream>
using namespace std;
int factorial(int n){
    cout<<n<<" * "<<n-1<<endl;
    if(n<=1){
        return 1;
    }
    return n*factorial(n-1);
}
int main(){
  int n;
  cin>>n;
  
  cout<<factorial(n)<<endl;
  return 0;
}

  ## Static
  
  static keyword is used, variable or data members or functions can not be modified again. It is allocated for the lifetime of program. Static functions can be called directly by using class name. Static variables are initialized only once. Compiler persist the variable till the end of the program.
  
  ## Class
  
  Class is a user-defined datatype that contain its own data members and member functions. The member functions and data members can be accessed with the help of objects. It is the primary concept of object-oriented programming. A class is used to organize information or data so a programmer can reuse the elements in multiple instances.
## Object
  An object is an instance of a class. As already mentioned above, all the data members and member functions of the class can be accessed with the help of objects.

  ## Inheritance
  
  Inheritance is a mechanism of reusing and extending existing classes without modifying them, thus producing hierarchical relationships between them. Inheritance is almost like embedding an object into a class.

  ## indexing in dbms
  
Indexing is a data structure technique to efficiently retrieve records from the database files based on some attributes on which the indexing has been done. Indexing in database systems is similar to what we see in books.
  
 ## find the name proximity of the given two names c++
  Ans: https://brainly.in/question/30128077
  
  ## palindrome
  
  A palindrome number remains the same if its digits are reversed i.e its value does not change.
  
  ## Logic for palindrome in string in c++
  Ans:
  
  
  ## Find the largest three digit number from seven digit number in c++
  ## or Find the largest 3 digit no contained in a no
  
  ans:
  
  ## What is Inheritance? It's applicantions and implementation?
Inheritance allows programmers to create classes that are built upon existing classes, to specify a new implementation while maintaining the same behaviors (realizing an interface), to reuse code and to independently extend original software via public classes and interfaces.

 ## Primitive data types available in C++ are:
Integer.
Character.
Boolean.
Floating Point.
Double Floating Point.
Valueless or Void.
  
  ## Non primitive data types
  
  Non primitive data types can also be referred to as the data type that is derived from primary data types. Also, we use the non-primitive data types to store the group of values. Examples of the non-primitive data types are Array, structure, union, link list, stacks, queue etc.

  ## What is the precision for floating point numbers?
  
A float has 23 bits of mantissa, and 2^23 is 8,388,608. 23 bits let you store all 6 digit numbers or lower, and most of the 7 digit numbers. This means that floating point numbers have between 6 and 7 digits of precision, regardless of exponent.
  
## What is the average time complexity for Binary Search?

ans:  O(logN)
The dominant term is N * logN / (N+1) which is approximately logN. Therefore, Average Case Time Complexity of Binary Search is O(logN).
  
  ## dynamic memory allocation in c++ example
  Ans: 
  
 ## Advantages of Dynamic memory allocation
Data structures can grow and shrink according to the requirement. We can allocate (create) additional storage whenever we need them. We can de-allocate (free/delete) dynamic space whenever we are. done with them.
  
  ## How do you find the largest and smallest number in C++?
  Ans:
  
  ## What is malloc?

  The malloc() function stands for memory allocation. It is a function which is used to allocate a block of memory dynamically. It reserves memory space of specified size and returns the null pointer pointing to the memory location. The pointer returned is usually of type void.
  
  ## How do we do CRUD operations in DBMS? How to join two tables with foreign key?
  
  ans:
  
  In the relational databases, a foreign key is a field or a column that is used to establish a link between two tables.
In simple words you can say that, a foreign key in one table used to point primary key in another table.
  
  
 ## What is method overloading?
Method overloading is a form of polymorphism in OOP. Polymorphism allows objects or methods to act in different ways, according to the means in which they are used. One such manner in which the methods behave according to their argument types and number of arguments is method overloading.
  
 ## Find greatest digit and its two adjacent in a number
#include <iostream>
using namespace std;
bool valid(int x){
    if(x==0)return 1;
    if(x%10==(x/10)%10)return 0;
    return valid(x/10);
}
unsigned long long n;
int main() {
    cin>>n;
    n++;
    while(1){
        if(valid(n)){
            cout<<n;
            return 0;
        }
        n++;
    }
}
 
  
## Substrings of a given string

#include<bits/stdc++.h>
using namespace std;

void subString(string s, int n)
{
	for (int i = 0; i < n; i++)
		for (int len = 1; len <= n - i; len++)
			cout << s.substr(i, len) << endl;
}

int main()
{
	string s = "abcd";
	subString(s,s.length());
	return 0;
}
