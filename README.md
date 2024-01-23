import java.util.Scanner;
import java.util.Random;
public class Main
{
  public static void f1(int ageson1) 
  {
    int ageson2 = ageson1 - 10;
    int agedouther = ageson2 + 1;
    int agedouther2 = agedouther + 3;
    System.out.println("childern 1 age is: " + ageson1);
    System.out.println("childern 2 age is: " + agedouther2);
    System.out.println("children 3 age is: " + agedouther);
    System.out.println("children 4 age is: " + ageson2);
  }
  public static void f2(int num) 
  {
    int digit1=num/100;
    int digit2=(num%100)/10;
    int digit3=num/10%10;
    System.out.println(""+digit3+digit2+digit1);
  }
  public static void f3() 
  {
    Random r = new Random();
    int num = r.nextInt(40,101);
    int num1 = r.nextInt(40,101); 
    int num2 = r.nextInt(40,101); 
    if (num>num1 && num>num2)
      System.out.println(num);
    if (num1>num && num1>num2)
       System.out.println(num1);
    if (num2>num && num2>num1)
      System.out.println(num2);
  }
  public static void f4(String str1,String str2)
  {
    int size1 = str1.length();
    int size2 = str2.length();
    if (size1 > size2)
      System.out.println(str1);
    else
      System.out.println(str2);
    String str3=str1.substring(0,3);
    String str4=str2.substring(0,3);
    System.out.println(str3);
    System.out.println(str4);
    int dictionnary=str3.compareTo(str4);
    if (dictionnary>0)
      System.out.println(str3);
    else
      System.out.println(str4);
  }
  public static void main(String[] args)
  {
  f1(8);
  f2(123);
  f3();
  f4("noahd","liordk");
  }
}
