# Module-3-Discussion-Project
This is an assignment submission link for Module 3 Discussion

using System;

class Program
{
  static void Main()
  {
    //Create a TopLevel Object and output member value
    TopLevel.Nested.Foo1();
    //Create a second TopLevel Object and output member value
    Console.WriteLine("The x value of TopLevel Class Nested class Foo2 function is {0}",   TopLevel.Nested.Foo2());
  }
}

public class TopLevel
{
  static int x = 6;
  public class Nested 
  {
    public static void Foo1() { Console.WriteLine (TopLevel.x); }
    
    public static int Foo2() {
      TopLevel.x = 9;
      return TopLevel.x; }
  }
}
