# sdi-assignent
// program on abstract class and method.
package Assignment01;

abstract class Animal {
	abstract public void makeSound();

	public void eat() {
		System.out.println("I can eat.");
	}
}

class Dog extends Animal {
	public void makeSound() {
		System.out.println("Bark bark");
	}
	
}

public class AbstractDemo {
	public static void main(String[] args) {
		Dog d1=new Dog(); 
		d1.makeSound();
		d1.eat(); 
		}
}
Output:
Bark bark
I can eat.




**// program on setter and getter method**
package Assignment01;
class Person{
	private String name;
	public void setName(String name) {
		this.name=name;
	}
	public String getName() {
	return name; 
	}
}
 
public class SetGet {
	public static void main(String argvs[]) {
		Person ps = new Person();
		ps.setName("Pinaki");
		System.out.println("The name is:"+ps.getName());
	}
	

}
OUTPUT: The name is:Pinaki
    

**Prpgram on run time polymorphism**
class Bike{  
  public void run(){
  System.out.println("running");
  }  
 
}  
class Splendor extends Bike{  
  public void run(){
  System.out.println("running safely with 60km");
  }  
  
  public static void main(String args[]){  
    Bike b = new Splendor();  
    b.run();  
  }  
}  
Output:

running safely with 60km.
**program on multilevel inheritance**
class Car{
   public Car()
   {
	System.out.println("Class Car");
   }
   public void vehicleType()
   {
	System.out.println("Vehicle Type: Car");
   }
}
class Maruti extends Car{
   public Maruti()
   {
	System.out.println("Class Maruti");
   }
   public void brand()
   {
	System.out.println("Brand: Maruti");
   }
   public void speed()
   {
	System.out.println("Max: 90Kmph");
   }
}
public class Maruti800 extends Maruti{

   public Maruti800()
   {
	System.out.println("Maruti Model: 800");
   }
   public void speed()
   {
	System.out.println("Max: 80Kmph");
   }
   public static void main(String args[])
   {
	 Maruti800 obj=new Maruti800();
	 obj.vehicleType();
	 obj.brand();
	 obj.speed();
   }
}
Output:

Class Car
Class Maruti
Maruti Model: 800
Vehicle Type: Car
Brand: Maruti
Max: 80Kmph
**program on multiple inheritance unsupported**
interface Backend {

  // abstract class
  public void connectServer();
}
class Frontend {
  public void responsive(String str) {
    System.out.println(str + " can also be used as frontend.");
  }
}
class Language extends Frontend implements Backend {
  String language = "Java";
  public void connectServer() {
    System.out.println(language + " can be used as backend language.");
  }
  public static void main(String[] args) {
    Language java = new Language();
java.connectServer();
    java.responsive(java.language);
  }
}
Output

Java can be used as backend language.
Java can also be used as frontend.

**program to demonstrate method overloading**
class Calculate
{
  void sum (int a, int b)
  {
    System.out.println("sum is"+(a+b)) ;
  }
  void sum (float a, float b)
  {
    System.out.println("sum is"+(a+b));
  }
  Public static void main (String[] args)
  {
    Calculate  cal = new Calculate();
    cal.sum (8,5);      //sum(int a, int b) is method is called.
    cal.sum (4.6f, 3.8f); //sum(float a, float b) is called.
  }
}
OUTPUT

Sum is 13
Sum is 8.4
**program on stack operation using interface**
import java.util.*;
 
public class Main
{
    public static void main(String[] args) {
        //declare and initialize a stack object
        Stack<String> stack = new Stack<String>();
                stack.push("PUNE");
                stack.push("MUMBAI");
            stack.push("NASHIK");
                System.out.println("Stack elements:");
                //get an iterator for the stack
                Iterator iterator = stack.iterator();
                //traverse the stack using iterator in a loop and print each element
                while(iterator.hasNext()){
                        System.out.print(iterator.next() + " "); 
             
                }
    }
}
Output:

Stack elements:
PUNE MUMBAI NASHIK

  **program to calculate employee salary**
  class NetSalary
 {
	public static void main(String arg[])	
	{
	    double grossSalary=10000;
	    double incomeTax=1000; 
	    double	 providentFund=800;    
	    double professionalTax=500;
	    double netSalary=grossSalary-(incomeTax+providentFund+professionalTax);
	     System.out.println("Net Salary is="+netSalary);
                   }
}
  
Output:

Net Salary is=7700.0
  
  **Program to calculate area of the square**
import java.util.Scanner;
class SquareAreaDemo {
   public static void main (String[] args)
   {
       System.out.println("Enter Side of Square:");
       Scanner sc = new Scanner(System.in);
       int side = sc.nextInt();
       //Area of Square = side*side
       int area = side*side; 
       System.out.println("Area of Square is: "+area);
   }
}
Output:

Enter Side of Square:
2
Area of Square is: 4
  
  **Program on interface with adda() and sub() method**
 
  class Overload_Demo implements 
{
     public void add()
     {
          System.out.println("Addition of "+a+" and "+b+" is: "+(a+b));
     }
     public void sub()
     {
          System.out.println("Subtraction of "+a+" and "+b+" is: "+(a-b));
     }
     public static void main(String[] args)
     {
          Overload_Demo obj = new Overload_Demo();
          obj.add();
          obj.sub();
     }
}


Output:
addition of 50 and 30 is: 80
  substraction of 50 and 50 and 30 is: 20


