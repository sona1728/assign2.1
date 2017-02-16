For a,b,c,d,e,f,h please refer the images attached.

solution for g: 

The method should be overloaded with the same return type in order to
avoid ambiguity.
For example:
class A{
static int add(int a,int b){return a+b;}
static double add(int a,int b){return a+b;}
}
class B{
public static void main(String[] args){
System.out.println(Adder.add(11,11));//ambiguity
}}
In this code when compiled it will show error as:
Overloading3.java:3: error: method add(int,int) is already defined in class A
static double add(int a,int b){return a+b;}

To overcome this problem, method should be overloaded with the same return type.
