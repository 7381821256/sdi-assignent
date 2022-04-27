# sdi-assignent
// program on abstract class and method.
abstract class Animal {
abstract void makeSound();
public void eat() {
System.out.println("I can eat.");
}
}
class Dog extends Animal {
public void makeSound()
{
System.out.println("Bark bark");
}
}
class main {
public static void main(String[] args) {
Dog d1=new Dog();
d1.make sound();
d1.eat();
}
}abstract class Animal {
  abstract void makeSound();

  public void eat() {
    System.out.println("I can eat.");
  }
}
