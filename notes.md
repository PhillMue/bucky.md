#BUCKY VIDEOS

 ##VIDEO 15: USING METHODS WITH PARAMETERS
    Create a method containing the parameter, for example String name, in the other class. In the main class import the scanner utility so that the user can define the value of 'name'. Afterwards, to use the method call it in the main class.

   To input Strings use input.nextLine();. For example: String put = input.nextLine();
   
   Argument - any extra formation that a program needs to run. e,g (String name) in this case, 'name' is the argument.
   
##VIDEO 16: MANY METHODS AND INSTANCES
Public variables are able to be used from other classes whereas Private variables can only be used within a class.

Return types are normally used to determine what a method should return. If the method is not to return anything, then we use "void".
 
 Comment print function: system.out.printf(format, args): Format is replaced by a string with %s between the quotation marks. %s refers to the string variable being referred to in args.

Instance variable: A variable that's outside a method but inside a class.

 ##VIDEO 17: CONSTRUCTORS
 A constructor is a method with the same name as a class and is used to initialize variables as soon as you create an object. This allows you to avoid calling the setter method. To use it you enter the variable as you create the object within the parameter brackets.

Each object has its own set of variables.

##VIDEO 18:NESTED IF STATEMENTS
This is adding another 'if' conditional within the false statement of the first 'if' conditional. Both correct statements are run along with the program.

this statement is used when more than one option output is required.

##VIDEO 19: ELSE IF STATEMENT
This is a way of giving java many options for an 'if' statement. 'else if' is placed between the 'if' and 'else' statements and can be used multiple times. The statement is only run until the point where the condition is true.

Curly braces are not required in an 'else if' statement. Use when one option is required of many.

##CONDITIONAL OPERATORS
Example of a conditional operator is:
System.out.println(age > 50 ? "Old": "Young")

the question mark in the function makes it a boolean. If age is greater than 50, "Old" is printed. otherwise, "Young" is printed. The value on the left represents true and that on the right represents false.

##VIDEO 21: SIMPLE AVERAGING PROGRAM

import scanner is used when values need to be input when the program runs.

    IMPORT SCANNER
    Outside the class type: import.java.util.*;
Within the class create object : Scanner Scannerobj = new Scanner(System.in);*
 
Use a while loop. Within the loop set an int variable equal to Scannerobj.nextInt();. Accumulate the sum using the loop and find average using by dividing the total by by the number of integers input.

##VIDEO 22: FOR LOOPS

Structure: for(int x = 0; x>10; x++)

The first statement shows where the loop starts, the second here it ends and the third the increments/decrements the value of the counter undergoes.

##VIDEO 23: COMPOUND INTEREST PROGRAM(COMPOUNDING NUMBERS)

Set the variables: double amount, double principal and double rate. Rate and principal are specified.

Using the for loop set the time as a condition.

    USING POWERS

 Formula: MAth.pow(arg0, arg1).

      arg0 is the number or expression while arg1 is the power.

#VIDEO 24:DO WHILE LOOP
It executes the loop at least once even if the test condition is false unlike the while loop.

STRUCTURE: do{Statements}while(condition);

#VIDEO 25: MATH CLASS METHODS
Math.max(x, y); Gives the maximum of two numbers.

Math.min(x, y); Gives the minumum of two numbers.

Math.sqrt(x); Square root of a number.

Math.abs(x); Gives you the absolute value of a number(number always becomes positve).

Math.ceil(x); Rounds up the number.

#VIDEO 26:RANDOM NUMBER GENERATOR


Math.floor(x); Rounds down the number.

#VIDEO 26: RANDOM NUMBER GENERATOR

Import the random number generator utility and create an object of it.

     EXAMPLE

     import.java.util.Random;

 Random randomobj = new Random();
Calling the object prints numbers from 0 if the statement is typed as: number = randomobj.nextInt(range);.

One should instead type it as umber = 1 + randomobj.nextInt(range); to get the specified numbers in the range.

#VIDEO 27: INTRODUCTION TO ARRAYS

This is a variable that can store many values in it of the same data type.

Structure of an int array: int arrayname[ ]=new int[x];. Where x is equal to number of variables being stored.

Storage indexes start from 0. To store values use the indexes to replace x. For example: arrayname[0] =44;

To shorten amking an array use an initializer. For example: int arrayname[ ]={1,2,3,4,5};

#VIDEO 28:  CREATING AN ARRAY TABLE

    NOTE: "\ t" in a string means a tab of about five spaces.
       arrayname.length store the number of values inyour array.
       
Print "index" and "value" first with a tab (\t) then print the indexes and values of the array using a loop.

#VIDEO 29: SUMMING ELEMENTS OF ARRAYS

Create an array containing numbers and a sum variable initialized as 0;

Using a for loop add array values to the sum.

**NOTE: Use arrayname.length**
#VIDEO 30: ARRAY ELEMENTS AS COUNTERS

Import random utility and create its object.

Create an array to store the frequency at which a number appears. Afterwards, use a for loop to input the frquency.

Formula in loop: ++arrayname[1+randomobj.nextInt(x)];. Where x is equal to the range of numbers available to the random utility.

Print element and frequency.

Since elements are the numbers 1-6,use another for loop with x initialized as 1 and ending as arraynane.length to printthe actual values of elements and their frequencies.
#VIDEO 31: ENHACED FOR LOOP

To use this initialze an array then start a for loop statement.

Structure: For(int x: arrayyname)
#VIDEO 32: ARRAYS IN METHODS

First initialize an array(int y[]) within the main method.

Afterwards create a method int the class with a parameter of the same data type(int x[]).Use a for loop to add a number to each element of this array.For example: x[counter]+=5.

Call the method in the array within the main method to add 5 to each element within array y using: methodName(y);
#VIDEO 33: MULTIDIMENSIONAL ARRAYS

These are arrays which contain more than a single array within them. They are use to create tables and store coordinates.

For example: int array[][]={{1,2,3,4,5}{6,7,8,9,0}}

To call elements use array index and element index while remembering that indexes start from 0.
#VIDEO 34: TABLE FOR MULTIDIMENSIONAL ARRAYS

To create tables showing all the the data in the multimensional arrays, create a method with an array as its parameter and containing two for loops(one is nested) to display the rows and columns. The first loop loops to the length of the first index of multidimensional array in the parameters while the second loops using both indexes.

    EXAMPLE

    public static void table(int x [][]){
    for (int row=0; row<x.length;row++){
       for(int column=0;column<x[row].length;column++){
          System.out.println(x[row][column]);
          }
       }
    }
Afterwards call this in the main method,for example: table(arrayname);, to print the array as a table.
#VIDEO 35: VARIABLE LENGTH ARGUMENTS

This is used when the number of variables being input is unknown. To use it you type: int...variablename.

To calculate average using this do:

   public static int average(int...varname){
      int sum=0;
      for(intx:varname){
         sum+=x;
      }
      return sum/varname.length;
   }
Afterwards call this method in the main method while inputting the required number as parameters. For example: average(1,2,3,4,5,6);
#VIDEO 36: 24 HOUR TIME CLASS

Create a class with the private variables hour, minute and second. Within the class create the setTime method with parameters representing the aforementioned variables.

In the setter equate the private variables to the parameters while inputting conditions. Replace 24 with 60 for minute and second. The last part of the conditional sets default value as 0;

 Example
 hour = ((h>=0 && h<24 ? h : 0)
For the 24 hour system create a method containing the statement below:

public String fullHours(){
return String.format("%02d:%02d:%02d", hour, minute, second);
}
%02d represents setting the numbers shown for time for each unit to two integers.
#VIDEO 37: 12 HOUR TIME CLASS

Create another method in the time class.

  public String halfHours(){
     return String.format("%d:%02d:%02d %s", ((hour==0 || hour==12) ? 12: hour%12), minute, second, (hour < 12? "AM":"PM"));
  }
Use the setter in the main method of the main class to set the time after creating an object.

#VIDEO 38: PUBLIC, PRIVATE AND THIS

Private prevents use of variables outside a class.

Public allows use of variables outside a class.

.this prefixed to a variable ensures that variables refered to in a method are those within the method instead of variables outside of a method if the have the same name.
#VIDEO 39: MULTIPLE CONSTRUCTORS

This is done using different numbers of arguments for each constructor created in a class.

This allows the user to enter specific sets of information to perform specific different tasks.
#VIDEO 40: SET AND GET METHODS

These enable you to set and get private variables.
#VIDEO 46: STATIC

This modifier enables you to share values with all objects in a class.

For example, members in a club initialized as a private int equal to 0. If the value of members in the constructor is set to member++; each object creation increases the members variable automatically.

#VIDEO 47: MORE ON STATIC

Use a static get method to call static variables in a class.

With static type you can use a class instead of an object to call the static method; since static methods are shared among all objects.

#VIDEO 48: FINAL

Always put constants in capital letters. Final type variables become constants(they cannot change after being set).

You can initialize final type variables in constructors.

#VIDEO 49: INHERITANCE

Syntax: public class child extends parent{}

Using the extends keyword one can get all methods within a parent class without retyping them.

Creating a method again in child class overrides the inherited methods.

A child of a child class inherits public methods of its parent class and its parent's class parent class.
#VIDEO 50: GUI

The method used to do this is to use the inbuilt class JOption.

  Import the class using: import javax.swing.JOptionPane;
EXAMPLE OF USAGE: Creating a program which take two numbers separately and shows your sum.

  public static void main(String[] args){
  String number1 = JOptionPane.showInputDialog("Enter first number");
  String number2 = JOptionPane.showInputDialog("Enter second number");

  int num1 = Integer.parseInt(number1);
  int num2 = Integer.parseInt(number2);
  int sum = num1 + num2;

  JOptionPane.showMessageDialog(null, "The answer is " + sum, "the title", JOptionPane.PLAIN_MESSAGE);}
  
#VIDEO 51: GUI WITH JFRAME

      This is to build a program which inherits the looks and feel of the OS on which it is run.

      From class without main method

        import java.awt.FlowLayout;      To avoid programming a layout.
        import javax.swing.JFrame;       Basic window layout
        import javax.swing.JLabele;      A line a text; allows you to do simple images.

         public class classname extends JFrame{
         private Jlabel item1;

          public classname(){
          super("title");                              Title being used
          setLayout(new FlowLayout ());                Setting the layout

          item1 = new JLabel("This is a sentence");    A sentence
          item1.setToolTipText("shows up on hover");   Appears on hovering
          }
           }


   From class with main method

   import javax.swing.JFrame;

   main method(){
   classname obj new classname();
   obj.setDefaultCloseOperation(JFrame.EXIT_ ON _CLOSE);
   obj.setSize(275,189);
   obj.setVisible(true);
   }

































