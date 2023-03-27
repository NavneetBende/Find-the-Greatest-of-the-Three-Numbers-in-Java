# Find-the-Greatest-of-the-Three-Numbers-in-Java

Given Three integer inputs num1, num2 and num3, the objective is ti write a code to Find the Largest of the Three Numbers in Java Language. In this article we will see a  Java program to Find Greatest of three numbers. We will use if else conditions and ternary operator too to find the same. Here are some of the methods to solve the above mentioned problem,

Method 1: Using if-else Statements 2
Method 2: Using if-else Statements 2
Method 3: Using Ternary Operator
We’ll discuss the above mentioned methods in the sections below in depth.

Method 1: Using if-else Statements 1
Java Code
Run
public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

    //checking if num1 is greatest
    if (num1 >= num2 && num1 >= num3)
        System.out.println (num1 + " is the greatest");

    //checking if num2 is greatest
    else if (num2 >= num1 && num2 >= num3)
        System.out.println (num2 + " is the greatest");

    //checking if num2 is greatest
    else if (num3 >= num1 && num3 >= num2)
        System.out.println (num3 + " is the greatest");
  }
}
Output
30 is the greatest
While loop in C
Method 2: Using if-else Statements 2
Java Code
Run
public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

    //comparing num1 with other numbers
    if ((num1 >= num2) && (num1 >= num3))
        System.out.println (num1 + " is the greatest");

    //checking if num2 is greatest
    else if (num2 >= num1 && num2 >= num3)
        System.out.println (num2 + " is the greatest");

    // num3 has to be greatest then if not above
    else
        System.out.println (num3 + " is the greatest");
  }
}

Output
30 is the greatest
Method 3: Using Ternary Operator
In this method we use the knowledge of Ternary Operators in Java.

Ternary Operator Syntax
( Condition ) ? ( if True : Action ) : ( if False : Action )

Java Code
Run


public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

     int temp, result;    
    
    // find the largest b/w num1 and num2 & store in temp
    temp = num1>num2 ? num1:num2;
    
    // find the largest b/w temp and num3 & finally printing it
    result = temp>num3 ? temp:num3;  
    System.out.println (result + " is the greatest");
  }
}

Output
30 is the greatest
