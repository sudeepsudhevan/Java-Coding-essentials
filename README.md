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

