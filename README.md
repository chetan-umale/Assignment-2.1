Q1-Write a Java code with the class name, “acad,” and a method called “main.”Hard code the program with two integers and print the sum of     those two integers.


public class acad {
	public static void main(String args[])
	{
		int a=4,b=7;
		int c=a+b;
		System.out.println(c);
	}

}


Q2-Rewrite the above code, wherein the inputs are provided by the user at runtime and the output is printed.


import java.util.Scanner;


public class acad {
	public static void main(String args[])
	{
		int a,b;
		Scanner s = new Scanner(System.in);
		System.out.println("Enter 2 numbers :");
		a=s.nextInt();
		b=s.nextInt();
		int c=a+b;
		System.out.println(c);
	}

}


Q3-Write a program with the method name, “sum()” that accepts two parameters from the user and print the sum of those two numbers. The
output format should be:
First number is:
Second number is:
Sum is:




import java.util.Scanner;


public class acad {
	public static void main(String args[])
	{
		int a,b;
		Scanner s = new Scanner(System.in);
		
		a=s.nextInt();
		b=s.nextInt();
		acad obj = new acad();
		int c=obj.sum(a, b);
		System.out.println("First number is : "+a);
		System.out.println("Second number is : "+b);
		System.out.println("Sum is :"+c);
	}
	
	public int sum(int x,int y)
	{
		return x+y;
	}

}



Q4-Write a program to accept two numbers from “stdin” and find all the odd as well as even numbers present in between them.


import java.util.Scanner;


public class acad {
	public static void main(String args[])
	{
		int a,b;
		Scanner s = new Scanner(System.in);
		
		a=s.nextInt();
		b=s.nextInt();
		
		System.out.println("odd numbers : ");
		
		for(int i=a+1;i<b;i++)
		{
			if(i%2!=0)
			{
				System.out.print(i+" ");
			}
		}
		
		System.out.println("\neven numbers : ");
		
		for(int i=a+1;i<b;i++)
		{
			if(i%2==0)
			{
				System.out.print(i+" ");
			}
		}
		
	}
	
	

}


Q5-e. Joe is scared to go to school. When her dad asked for the reason, Joe said
that she was unable to complete the task given to her by her teacher. The
task was to find the “first 10 multiples” of the number entered from
“stdin”. 


import java.util.Scanner;


public class acad {
	public static void main(String args[])
	{
		int a,b;
		Scanner s = new Scanner(System.in);
		System.out.println("Input :");
		a=s.nextInt();
		
		
		
		System.out.println("output :" );
		for(int i=1;i<=10;i++)
		{
			
			
				System.out.println(a+" x "+i+" = "+a*i);
			
		}
		
		
		
	}
	
	

}





Q6-Write a program consisting the method “sum()” and demonstrate the
concept of method overloading using this method.




import java.util.Scanner;


public class acad {
	public static void main(String args[])
	{
		int a,b,c;
		
		
		acad obj = new acad();
		
	
		Scanner s = new Scanner(System.in);
		System.out.println("enter 2 numbers");
		a=s.nextInt();
		b=s.nextInt();
		
		System.out.println("sum 1 : " +obj.add(a, b) );
		
		System.out.println("enter 3 numbers");
		a=s.nextInt();
		b=s.nextInt();
		c=s.nextInt();
		
		
		System.out.println("sum 2 : "+obj.add(a, b, c) );
		
		
	}
	
	
	public int add(int x,int y)
	{
		return x+y;
	}
	
	public int add(int x,int y,int z)
	{
		return x+y+z;
	}	

}



