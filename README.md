# Java Coding

1. **Add Two numbers**

```
import java.util.Scanner;

public class HelloSample {

	
	public static void main(String ar[]) {
		
		
		Scanner s=new Scanner(System.in);
		
		System.out.println("Enter 2 number");
		
		int a=s.nextInt();
		int b=s.nextInt();
		
		int c=a+b;
		
		System.out.println("Result: "+c);
	}
}
```

2. **If sample**
```
import java.util.Scanner;

public class IfSample {
	
	public static void main(String a[]) {
		
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter a number");
		
		int num=sc.nextInt();
		
		if(num<0) {
			System.out.println("Number is negative");
		}else {
			System.out.println("Number is positive");
		}
				
		}
	
}
```

3. **Function Sample**
```
import java.util.Scanner;

public class FunctionSample {
	public static void main(String a[]) {
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter two numbers");
		
		int num1=sc.nextInt();
		int num2=sc.nextInt();
		
		int result=sum(num1,num2);
		
		System.out.println("Result is:"+result);
		
		
	}

	
	static int sum(int a,int b) {
		int s=a+b;
		return s;
	}
	
}
```

4. **Add Two Array**
```
import java.util.Scanner;

public class Addtwodimen {
	
	public static void main(String a[]) {
		int[][] array1=new int[3][3];
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the size of arrays");
		
		int size=sc.nextInt();
		
		
		
		
		for(int i=0;i<3;i++) {
			for(int j=0;j<3;j++) {
				array1[i][j]=sc.nextInt();
			}
			
			System.out.println();
		}
		
		int[][] array2=new int[size][size];
		
		for(int i=0;i<3;i++) {
			for(int j=0;j<3;j++) {
				array2[i][j]=sc.nextInt();
			}
			System.out.println();
		}
		
	}
	

}
```

5. **Class Sample**

	  * file: `Sample.java`
	  ```
	  public class Sample {
	  	
	  	int a;
	  	int b;
	  	
	  	void display() {
	  	System.out.println("a: "+a+"      b:"+b);
	  	}
	  }
	  ```
	
	  * file: `Hello.java`
	  ```
	  public class Hello {
	  	
	  	public static void main(String a[]) {
	  		
	  		
	  		Sample s1=new Sample();
	  		Sample s2=new Sample();
	  		
	  		s1.a=20;
	  		s2.a=50;
	  		s1.b=100;
	  		s2.b=200;
	  		
	  		s1.display();
	  		s2.display();
	  		
	  	}
	  
	  }
	```

6. Class Sample Add two numbers

	* file: `Sum.java`
	
	```
	public class Sum {
		
		
		int c;
		
		
		void calculate(int k,int m) {
			c=k+m;
		}
	
		void displaySum() {
			System.out.println("Sum is:"+c);
		}
		
	}
	```
	
	* file: `Sample.java`
	
	```
	import java.util.Scanner;
	
	public class Sample {
		public static void main(String ar[]) {
			
			
			Scanner a=new Scanner(System.in);
			System.out.println("Enter 2 number");
			
			int num1=a.nextInt();
			int num2=a.nextInt();
	
			
			Sum s=new Sum();
			
			s.calculate(num1, num2);
			s.displaySum();
		}
	
	}
	```

7. Prime numbers
```
import java.util.Scanner;

public class PrimeNo {
	public static void main(String ar[]) {
		
		Scanner a=new Scanner(System.in);
		System.out.println("Enter a number: ");
		
		int num1=a.nextInt();
		int flag=0;
		
		
		for(int i=0;i<num1/2;i++) {
			if(num1%2==0) {
				flag=1;
				break;
			}
		}
	
		if(flag==0) {
			System.out.print("Number " +num1+ " is a Prime number");
		}else {
			System.out.print("Entered number " +num1+ " is not a Prime number");
		}
		
	}

}
```

8. **Math Operations**

	* file: `Operations.java`
	
	```
	public class Operations {
		
		void addition(int a,int b) {
			int c;
			c=a+b;
			System.out.println("Result:"+c);
			
		}
		
		
		void substraction(int a,int b) {
			int c;
			c=a-b;
			System.out.println("Result:"+c);
		}
		
		
		void multiplicatio(int a,int b) {
			int c;
			c=a*b;
			System.out.println("Result:"+c);
		}
		
		
		void division(int a,int b) {
			int c,r;
			c=a/b;
			r=a%b;
			System.out.println("quotient is:"+c+"  remainder is:"+r);
		}
	
	}
	```
	
	* file: `Sample.java`
	
	```
	import java.util.Scanner;
	
	public class Sample {
		public static void main(String ar[]) {
			
			
			Scanner a=new Scanner(System.in);
			System.out.println("Enter 2 number: ");
			
			int num1=a.nextInt();
			int num2=a.nextInt();
			
			
			Operations s=new Operations();
			System.out.println("1 for Addition \n2 for Substraction \n3 for Multiplication \n4 for Divison \nEnter a choice from above: ");
			int choice=a.nextInt();
			
			switch(choice) {
			case 1:
				s.addition(num1,num2);
				break;
			case 2:
				s.substraction(num1, num2);
				break;
			case 3:
				s.multiplicatio(num1, num2);
				break;
			case 4:
				s.division(num1, num2);
				break;
			default:
				System.out.println("Invalid Entry");
			}
		
		}
	}
	```   

9. **Static Sample**
```
public class Hello {
	 int a=10;
	static int b=20;
	public static void main(String hai[]) {
		
		Hello h=new Hello();
		Hello h1=new Hello();
		System.out.println(h.a);
		h.hello();
		
		h.b=50;
		
		h.a=100;
		
		h1.b=100;
		
		h1.a=1500;
		
		b=2000;
				
		hey();
		
		System.out.println("h.a "+h.a);
		System.out.println("h.b "+h.b); //b is static variable9
		System.out.println("h1.a "+h1.a);
		System.out.println("h1.b "+h1.b);
		System.out.println(b);
	}
	
	
	void hello() {
		
		System.out.println("hello "+a);
		
	}
	static void hey() {
		System.out.println("hey "+b);
	}
	
}
```

10. **Three Class Sample**

	* file: `Final.java`
	
	```
	public class Final {
		void displayFinal() {
			System.out.println("Welcm to me");
		}
	
	}
	```
	
	* file: `First.java`
	
	```
	public class First {
		void displayFirst() {
			Final f=new Final();
			f.displayFinal();
		}
	
	}
	```
	
	* file: `Hello.java`
	
	```
	public class Hello {
		public static void main(String ar[]) {
			First f=new First(); 
				f.displayFirst();
			
		}
	
	}
	```

11. **Construct Sample**

	* file: `Sample.java`
	  
	```
	public class Sample {
		Sample(){
			System.out.println("This is a construct");
		}
	
	}
	```
	
	* file: `Sample.java`
	
	```
	public class Hello {
		public static void main(String ar[]) {
			Sample s=new Sample();
			
			
			Hello h=new Hello();
			
		}
		
		
		Hello(){
			System.out.println("Hello ");
		}
	
	}
	```  

12. **This Sample**

	* file: `Sample.java`
	
	```
	public class Sample {
		int a=25,b=35;         // global variable construct
		
		
		Sample(int a,int b){   // local variable inside construct
			
			this.a=a;
			this.b=b;
			
			
			System.out.println(this.a+" "+this.b);  
			
			
		}
	
	}
	```
	
	* file: `Hello.java`
	
	```
	public class Hello {
		public static void main(String[] args) {
			Sample s=new Sample(10,25);
		}
	
	}
	```    

13. **Inheritance Sample**

	* file: `A.java`
	
	```
	public class A {
		int a;
		void displayA() {
			System.out.println("This is A ");
		}
	
	}
	```
	
	* file: `B.java`
	
	```
	public class B extends A {
		int num;
		
		void DisplayB() {
			System.out.println("This is B");
		}
	
	}
	```
	
	* file: `Sample.java`
	
	```
	public class Sample {
		
		public static void main(String[] args) {
			B b=new B();
			b.displayA();
			b.DisplayB();
		}
	
	}
	```

14. **Inheritance Constructor**

	* file: `A.java`
	
	```
	public class A {
		
		A(){
			System.out.println("It is A");
		}
	
	}
	```
	
	* file: `B.java`
	
	```
	public class B extends A {
		B(){
			System.out.println("it is B");
		}
		
		
		
		public static void main(String[] args) {
			B b=new B();
		}
			
	// here initially execute constructor in base class(Class A) then the constructor in the child class(Class B)
	
	}
	```   

15. **Super Sample**

	* file: `A.java`
	
	```
	public class A {
		
		int a;
		
		void display() {
			System.out.println("it is A");
			
		}
		
		
		A(){
			System.out.println("it is a A constructor");}
		
		A(int a){
			System.out.println("it is argument construct A");
		}
	
	}
	```
	
	* file: `B.java`
	
	```
	public class B extends A {
		
		int a;
		
		
		B(){
			System.out.println("It is a B constructor");
		}
		
		
		B(int a){
			//  super(10); super  should be first statement in method
			System.out.println("it is argument constructor B");
			
		}
		
		void display() {
			
			
			System.out.println("it is B");
			
			a=20;
			
			super.a=30;
			
			int c=a+super.a;
			
			System.out.println(c);
			
		}
		
		void baseDisplay() {
			super.display();
		}
		
		
		public static void main(String[] args) {
			B b=new B(10);
			
			//b.display();
			
			//b.baseDisplay();
		}
	
	}
	```

16. **Abstract Sample**

	* file: `TextScanner.java`
	
	```
	public class TextScanner {
		
		Hello obj;
		
		public TextScanner(Hello ob){
			
			this.obj=ob;	
			
		}
		void scan() {
			// code for scan
			
			String text="Scanned text";
			obj.onText(text);
			
			
			
		}
	
	}
	```
	
	* file: `abstract.java`
	  
	```
	public abstract class Hello {
		
		abstract void onText(String text);
	
	}
	```
	
	* file: `Sample.java`
	  
	```
	public class Sample extends Hello {
	
		@Override
		void onText(String text) {
			
			System.out.println(text);
			// TODO Auto-generated method stub
			
			
			
			
		}
		
		Sample(){
			TextScanner ts=new TextScanner(this);
			ts.scan();
			
			
		}
		
		
		
		public static void main(String[] args) {
			
			Sample s=new Sample();
			
		}
		
	}
	```

17. **Thread Sample**

	* file: `ThreadSample.java`
	
	```
	public class ThreadSample extends Thread {
		
		@Override
		public void run() {
			// TODO Auto-generated method stub
			super.run();
			
			for(int i=0;i<10;i++) {
				System.out.println("Thread count"+i);
				
				
				try {
					Thread.sleep(1000);
				} catch (InterruptedException e) {
					// TODO: handle exception
					
					e.printStackTrace();
				}
			}
			
		}
		
	}
	```
	
	* file: `Hello.java`
	
	```
	public class Hello {
		
		public static void main(String[] args) {
			ThreadSample st=new ThreadSample();
			
			st.start();
			ThreadSample st1=new ThreadSample();
			st1.start();
			
			ThreadSample st2=new ThreadSample();
			
			
			st2.start();
		}
	}
	```


     
