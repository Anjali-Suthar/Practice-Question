Ques1:fibonacci Series
class Main{
  public static void main(String[] args){
    int a=0,b=1,c=0;
    for(int i=0;i<10;i++){
      c=a+b;
      System.out.println(c);
      a=b;
      b=c;
    }
  }
}


Quest2:
import java.util.*;
class Main{
  public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
    System.out.println("Enterr the first number");
    int a = sc.nextInt();
    System.out.println("Enter the second number");
    int b = sc.nextInt();
    System.out.println("Enter the third number");
    int c = sc.nextInt();
    int[] arr = {a,b,c};
    int sum = 0;
   for(int i=0;i<arr.length;i++){
     sum = sum + arr[i];
   }
     System.out.println("Sum of number is " + sum);
     int avg = sum/arr.length;
     System.out.println("Average is " + avg);

    }
  }


  Quest3:
class Vehicle{
  String make;
  String model;
  int year;
}
class car extends Vehicle{
  String fuel;
  car(String make,String model,int year,String fuel){
    this.make=make;
    this.model=model;
    this.year=year;
    this.fuel=fuel;
  }
}
class Main{
  public static void main(String[] args){
    car c=new car("Toyota","Corolla",2020,"Petrol");
    System.out.println(c.make);
    System.out.println(c.model);
    System.out.println(c.year);
    System.out.println(c.fuel);
  }
}


Quest4:
interface Drawable{
  void draw();
}
class Circle implements Drawable{
  public void draw(){
    System.out.println("CIRCLE");
  }
}
class Square implements Drawable{
  public void draw(){
    System.out.println("SQUARE");
  }
}

abstract class Shape{
  public void draw(){
    System.out.println("SHAPE");
  }
}

class Main{
  public static void main(String[] args){
    Drawable d=new Circle();
    d.draw();
    Drawable d1 = new Square();
    d1.draw();
  
  }
}


Quest5:
abstract class Geometric{
  abstract void area();
  abstract void perimeter();
}
class Circle extends Geometric{
 private double radius;
  // final double pi = 3.14;
  Circle(double radius){
    this.radius=radius;
  }
  public void double area(){
    return 3.14*radius*radius;
  }
  public void double perimeter(){
    return 2*(3.14)*radius;
  }
}
class Rectangle extends Geometric{
  double length;
  double breadth;
  Rectangle(double length,double breadth){
    this.length = length;
    this.breadth = breadth;
  }
  public void double area(){
    return length*breadth;
  }
 public void double perimeter(){
    return 2*(length+breadth);
  }
}
class Main{
  public static void main(String[] args){
    Geometric g = new Circle(5);
    g.area();
    g.perimeter();
    Geometric g1 = new Rectangle(5,6);
    g1.area();
    g1.perimeter();
  }
}



   
