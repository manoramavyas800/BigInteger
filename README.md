# BigInteger
//print fibonacci.
import java.math.BigInteger;
import java.util.Scanner;

public class Recursion {
    public static BigInteger fibonacci(int n) {
        // code here
        BigInteger a=new BigInteger("0");
        BigInteger b=new BigInteger("1");
        BigInteger c;
        for(int i=2; i<=n; i++) {
            c = a.add(b);
            a = b;
            b = c;
        }
        return b;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t=sc.nextInt();
        BigInteger n= fibonacci(t);
        System.out.println(n);
    }
}
//print factorial.

import java.math.BigInteger;
import java.util.Scanner;

public class Recursion {
   static BigInteger factorial(int n) {
       BigInteger a = new BigInteger("1");
       for (int i = 1; i <= n; i++) {
           a = a.multiply(BigInteger.valueOf(i));
       }
       return a;
   }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t=sc.nextInt();
        BigInteger a =  factorial(t);
        System.out.println(a);
    }
}
