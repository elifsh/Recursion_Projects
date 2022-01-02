# Recursion_Projects
Fırat University Recursion_Projects

### Kendisine parametre olarak gelen değerin faktöriyelini döndüren recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    public static int factorial(int a) {
        if (a == 0) {
            return 1;
        } else {
            return a*factorial(a-1);
        }        
    }
    public static void main(String[] args) {
        Random r = new Random();
        int num = r.nextInt(20);
        System.out.println("Number: " + num);
        System.out.println("Factorial of number: " + factorial(num));
    }
}
```
### Kendisine parametre olarak gelen pozitif tam sayıya kadar olan tamsayıları toplayan recursive methodu yazınız.
```java
import java.util.Random;
public class Main {
    public static int sum(int a) {
        if (a == 0) {
            return 0;
        } else {
            return a + sum(a-1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int num = r.nextInt(100)+1;
        System.out.println("Number: " + num );
        System.out.println("Sum Number: " + sum(num));
    }
}
```
### Kendisine parametre olarak gelen sayının kaç basamaklı olduğunu hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    public static int sum(int a) {
        if (a>=0 && a<=9) {
            return 1;
        } else {
            return 1 + sum(a/10);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int num = r.nextInt(100000)+1;
        System.out.println("Number: " + num );
        System.out.println("Number of digits: " + sum(num));
    }
}
```
### Kendisine parametre olarak gelen a ve b sayısını a^b cinsinde hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    public static int a_power_b(int a, int b) {
        if (b == 0) {
            return 1;
        } else {
            return a*a_power_b(a, b-1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int a = r.nextInt(10)+1;
        int b = r.nextInt(10)+1;
        System.out.println("Number: " + a +" || "+"Power: " + b );
        System.out.println("a power b: " + a_power_b(a,b));
    }
}
```
### Kendisine parametre olarak gelen sayı kadar adınızı yazdıran recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    public static String print_name(int a) {
        if (a == 0) {
            return "";
        } else {
            return "Elif\n"+print_name(a-1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int a = r.nextInt(10)+1;
        System.out.println("Number: " + a);
        System.out.println(print_name(a));
    }
}
```
### Kendisine parametre olarak gelen a sayısına karşılık gelen fibonacci dizi elemanını hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    static int temp = 0;
    public static int fibonacci(int i) {
        if (i==0 || i == 1) {
            return i;
        } else {
            return fibonacci(i-1)+fibonacci(i-2);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int i = r.nextInt(40)+1;
        System.out.println("Number: " + i);
        System.out.println("Fib: " + fibonacci(i));
    }
}
```
