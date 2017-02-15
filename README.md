# D2a1

a.

public class acad {
	public static void main(String[] args){
		int a=5;                              //assigning value to integer a
		int b=10;                              //assigning value to integer b
		System.out.println(a+b);             //Displaying the result sum
	}
}


b.

import java.util.Scanner;
public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int a=sc.nextInt();                //accepting value of first integer from user 
		int b=sc.nextInt();                //accepting value of second integer from user
		System.out.println(a+b);          //displaying the sum
	}
}

c.

import java.util.Scanner;
public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int a=sc.nextInt();         //accepting value of first integer from user
		int b=sc.nextInt();        //accepting value of second integer from user
		System.out.println("First number is:"+a);
		System.out.println("Second number is:"+b);
		sum(a,b);
	}
	public static void sum(int a,int b){
		System.out.println("Sum is:"+(a+b));
	}//method for calculating and displaying the sum
}

d.

import java.util.ArrayList;
import java.util.Scanner;


public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int a=sc.nextInt();            //accepting value of first integer from user
		int b=sc.nextInt();            //accepting value of second integer from user
		ArrayList<Integer> odd=new ArrayList<Integer>();       
		ArrayList<Integer> even=new ArrayList<Integer>();
		for(int i=a;i<=b;i++){
			if(i%2==0)
				even.add(i);               //Storing even numbers in arraylist
			else 
				odd.add(i);                //Storing odd numbers in arraylist
				
		}System.out.println("Odd numbers are:\n");
		for(int i:odd)
			System.out.print(i+" ");
		System.out.println("\nEven numbers are:\n");
		for(int i:even)
			System.out.print(i+" ");
		
		
	}
}



e.
import java.util.Scanner;

public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();                                     //accepting the number
		System.out.println("Input: "+n);
		System.out.println("O/p:");
		for(int i=1;i<=10;i++){
			System.out.println(n+" * "+i+" = "+(n*i));            //displaying table of given number
		}
		
		
	}
}



f.

import java.util.Scanner;


public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int a=sc.nextInt();       //Accepting 3 numbers from the user
		int b=sc.nextInt();
		int d=sc.nextInt();
		sum(a,b);
		sum(a,b,d);
	}
  // method overloading
	public static void sum(int a,int b){
		System.out.println("Sum of first 2 numbers is:"+(a+b));
	}
	public static void sum(int a,int b,int d){
			System.out.println("Sum of all 3 numbers is:"+(a+b+d));
	}
}


g.
The method should be overloaded with the same return type in order to avoid ambiguity.
For example,
class A{  
static int add(int a,int b){return a+b;}  
static double add(int a,int b){return a+b;}  
}  
class B{  
public static void main(String[] args){  
System.out.println(Adder.add(11,11));//ambiguity  
}}  
In this when code is compiled it will show error as:
Overloading3.java:3: error: method add(int,int) is already defined in class A
static double add(int a,int b){return a+b;} 

To overcome this problem method should be overloaded with the same return type.










h.

import java.util.Arrays;
import java.util.Scanner;


public class acad {
	public static void main(String[] args){
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt(); //size of array
		int[] arr=new int[n];
		for(int i=0;i<n;i++){
			arr[i]=sc.nextInt();
		}
		Arrays.sort(arr);               //sorting array
		for(int i=arr.length-1;i>=0;i--){
			System.out.print(arr[i]+" "); // displaying sorted reverse ordered array elements
		}
	}
}


