SUM OF DIGITS:
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);           
        int a = Integer.parseInt(scan.nextLine());  
        int sum = 0;
        while(a > 0){
            int r = a % 10;
            sum = sum + r;
            a = a / 10;
      }
        System.out.println(sum);
        scan.close();
    }
}

OUTPUT:
5
5

INPUT FOR ALL DATATYPES:
import java.util.Scanner;
public class Main
{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);   
        byte p = scan.nextByte();
        short q = scan.nextShort();
        int r = scan.nextInt();
        float v = scan.nextFloat();
        long t = scan.nextLong();
        double u = scan.nextDouble();      
        scan.nextLine();                   
        String str1 = scan.nextLine();   
        String str2 = scan.nextLine();        
        char ch = scan.next().charAt(0);        
        System.out.println(p + " " + q); 
        System.out.println(r + " " + v); 
        System.out.println(t + " " + u);
        System.out.println(str1 + " " + str2);
        System.out.println(ch);   
        scan.close();
    }
}

OUTPUT:
10 20
30 40.5
200 300.76889
hello hello world 
h

REVERSE ORDER:
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);     
        int a = Integer.parseInt(scan.nextLine());  
        int rev = 0;   
        while(a > 0){
            int r = a % 10;
            rev = rev * 10 + r;
            a = a / 10;
        }
        System.out.println(rev);
        scan.close();
    }
}

OUTPUT:
123456
654321

PALINDROME:
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);    
        int a = Integer.parseInt(scan.nextLine());  
        int rev = 0;   
        int original = a;  
        while(a > 0){
            int r = a % 10;
            rev = rev * 10 + r;
            a = a / 10;
        }
        System.out.println("Reversed: " + rev);
        if(original == rev){
            System.out.println("Palindrome");
        } else {
            System.out.println("Not Palindrome");
        }
        scan.close();
    }
}

OUTPUT:
345678
Reversed:876543
Not Palindrome

PRIME FACTORS OF NUMBER:
import java.util.*;  
public class Main{
    public static void main(String[] args) {
        int number = 84; 
        System.out.print("Prime factors of " + number + " are: ");
        for (int i = 2; i <= number; i++) {
            while (number % i == 0) {
                System.out.print(i + " ");
                number = number / i;
            }
        }
    }
}

OUTPUT:
Prime factors of 84 are: 2 2 3 7 

COUNT:
import java.util.*;
public class Main{
    public static void main(String[] args) {
        int number = 84;
        int count = 0;  
        System.out.print("Prime factors of " + number + " are: ");
        for (int i = 2; i <= number; i++) {
            while (number % i == 0) {
                System.out.print(i + " ");
                number = number / i;
                count++;   
            }
        }
        System.out.println("\nTotal count of prime factors = " + count);
    }
}

OUTPUT:
rime factors of 84 are: 2 2 3 7 
Total count of prime factors = 4

PRIME NUMBER:
import java.util.*;
public class  Main{
    public static void main(String[] args) {
        int number = 29; 
        boolean isPrime = true;
        if (number <= 1) {
            isPrime = false;
        } else {
            for (int i = 2; i <= number / 2; i++) {
                if (number % i == 0) {
                    isPrime = false;
                    break;
                }
            }
        }
        if (isPrime) {
            System.out.println(number + " is a PRIME number");
        } else {
            System.out.println(number + " is NOT a prime number");
        }
    }
}

OUTPUT:
29 is a PRIME number

FACTORIAL:
import java.util.*;
public class Main{
    public static void main(String[] args) {
        int number = 5;   
        long factorial = 1;
        for (int i = 1; i <= number; i++) {
            factorial = factorial * i;
        }
        System.out.println("Factorial of " + number + " = " + factorial);
    }
}

OUTPTUT:
Factorial of 5 = 120

FIBONACCI SERIES:
import java.util.*;
public class Main{
    public static void main(String[] args) {
        int n = 10;  
        int first = 0, second = 1;
        System.out.println("Fibonacci Series for " + n + " terms:");
        for (int i = 1; i <= n; i++) {
            System.out.print(first + " ");
            int next = first + second;
            first = second;
            second = next;
        }
    }
}

OUTPUT:
Fibonacci Series for 10 terms:
0 1 1 2 3 5 8 13 21 34 



