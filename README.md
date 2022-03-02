# Recursion_Projects
Fırat University Recursion_Projects

| PRATİKLER |
|-----
| [PRATİK 1](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-de%C4%9Ferin-fakt%C3%B6riyelini-d%C3%B6nd%C3%BCren-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Faktöriyel Hesaplama |
| [PRATİK 2](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-pozitif-tam-say%C4%B1ya-kadar-olan-tamsay%C4%B1lar%C4%B1-toplayan-recursive-methodu-yaz%C4%B1n%C4%B1z) - Gauss Toplamı |
| [PRATİK 3](https://github.com/elifsh/Recursion_Projects/edit/main/README.md#kendisine-parametre-olarak-gelen-say%C4%B1n%C4%B1n-ka%C3%A7-basamakl%C4%B1-oldu%C4%9Funu-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Basamak Sayısı Bulma |
| [PRATİK 4](https://github.com/elifsh/Recursion_Projects/edit/main/README.md#kendisine-parametre-olarak-gelen-a-ve-b-say%C4%B1s%C4%B1n%C4%B1-ab-cinsinde-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Üslü Sayı Hesaplama |
| [PRATİK 5](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-say%C4%B1-kadar-ad%C4%B1n%C4%B1z%C4%B1-yazd%C4%B1ran-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Sayı Kadar İsim Yazdırma |
| [PRATİK 6](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-a-say%C4%B1s%C4%B1na-kar%C5%9F%C4%B1l%C4%B1k-gelen-fibonacci-dizi-eleman%C4%B1n%C4%B1-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Fibonacci Dizisi Yazdırma |
| [PRATİK 7](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-tamsay%C4%B1-dizisindeki-en-b%C3%BCy%C3%BCk-eleman%C4%B1n-indisini-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - En Büyük Elemanın İndisini Yazdırma |
| [PRATİK 8](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-tamsay%C4%B1n%C4%B1n-s%C4%B1ral%C4%B1-olup-olmad%C4%B1%C4%9F%C4%B1n%C4%B1-kontrol-eden-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Sıralı Dizi Kontrolü |
| [PRATİK 9](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-dizinin-simetrik-olup-olmad%C4%B1%C4%9F%C4%B1n%C4%B1-kontrol-eden-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Simetrik Dizi Kontrolü |
| [PRATİK 10](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-dizide-ka%C3%A7-tane-pozitif-tam-say%C4%B1-oldu%C4%9Funu-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Pozitif Tamsayı Sayacı |
| [PRATİK 11](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-dizide-ka%C3%A7-tane-k%C3%BC%C3%A7%C3%BCk-karakter-oldu%C4%9Funu-hesaplayan-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Küçük Karakter Sayacı |
| [PRATİK 12](https://github.com/elifsh/Recursion_Projects/edit/main/README.md#kendisine-parametre-olarak-gelen--diziyi-ters-%C3%A7eviriren-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Dizi Ters Çevirme|
| [PRATİK 13](https://github.com/elifsh/Recursion_Projects#kendisine-parametre-olarak-gelen-stringi-ters-%C3%A7eviren-recursive-fonksiyonu-yaz%C4%B1n%C4%B1z) - Kelime Ters Yazma |

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# :open_book: PRATİK 1	- Faktöriyel Hesaplama

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 2	- Gauss Toplamı

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 3	- Basamak Sayısı Bulma

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 4	- Üslü Sayı Hesaplama

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 5	- Sayı Kadar İsim Yazdırma

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 6	- Fibonacci Dizisi Yazdırma

## SORU :question:
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
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 7	- En Büyük Elemanın İndisini Yazdırma

## SORU :question:
### Kendisine parametre olarak gelen tamsayı dizisindeki en büyük elemanın indisini hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Arrays;
import java.util.Random;
public class Main {
    static int big = 0;
    public static int r_big_num(int []arr, int i) {
        if (i == arr.length) {
            return big;
        } else {
            if (arr[big] < arr[i]) {
                big = i;
            }
            return r_big_num(arr, i+1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int[]arr = new int[10];
        for (int i = 0; i < arr.length; i++) {
            arr[i] = r.nextInt(10)+1;
        }
        System.out.println(Arrays.toString(arr));
        System.out.println(r_big_num(arr, 1));
    }
}
``` 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 8	- Sıralı Dizi Kontrolü

## SORU :question:
### Kendisine parametre olarak gelen tamsayının sıralı olup olmadığını kontrol eden recursive fonksiyonu yazınız.
```java
import java.util.Arrays;
import java.util.Random;
public class Main {
    public static boolean array_sort_control(int[]arr, int i){
        if (i == arr.length-1) {
            return true;
        } else {
            if (arr[i]>arr[i+1]) {
                return false;
            } else {
                return array_sort_control(arr, i+1);
            }
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int[] arr = new int[5];
        for (int i = 0; i < arr.length; i++) {
            arr[i]=r.nextInt(100)+1;
        }
        System.out.println(Arrays.toString(arr));
        System.out.println(array_sort_control(arr, 0));
    }
}
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 9	- Simetrik Dizi Kontrolü

## SORU :question:
### Kendisine parametre olarak gelen dizinin simetrik olup olmadığını kontrol eden recursive fonksiyonu yazınız.
```java
import java.util.Arrays;
public class Main {
    public static boolean palindrome_arr(int[] arr, int i) {
        if (i == arr.length-1) {
            return true;
        } else {
            if (arr[i]!=arr[arr.length-i-1]) {
                return false;
            }
            return palindrome_arr(arr, i+1);
        }
    }
    public static void main(String[] args) {
        int[] arr = {1,0,0,1};
        System.out.println(Arrays.toString(arr));
        System.out.println(palindrome_arr(arr, 0));
    }
}
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 10	- Pozitif Tamsayı Sayacı

## SORU :question:
### Kendisine parametre olarak gelen dizide kaç tane pozitif tam sayı olduğunu hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Arrays;
import java.util.Random;
public class Main {
    static int temp = 0;
    public static int positive_num(int[] arr, int i) {
        if (i == arr.length) {
            return temp;
        } else {
            if (arr[i]>0) {
                temp++;
            }
            return positive_num(arr, i+1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int[] arr = new int[10];
        for (int i = 0; i < arr.length; i++) {
            arr[i]=r.nextInt(100)-10;
        }
        System.out.println(Arrays.toString(arr));
        System.out.println(positive_num(arr, 0));
    }
}
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 11	- Küçük Karakter Sayacı

## SORU :question:
### Kendisine parametre olarak gelen dizide kaç tane küçük karakter olduğunu hesaplayan recursive fonksiyonu yazınız.
```java
import java.util.Scanner;
public class Main {
    static int temp = 0;
    public static int small_num(char[]arr, int i) {
        if (i ==arr.length) {
            return temp;
        } else {
            if (arr[i]>=97 && arr[i]<=122) {
                temp++;
            }
            return small_num(arr, i+1);
        }
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Please enter your string: ");
        String str = sc.next();
        char[]ch = str.toCharArray();
        System.out.println(small_num(ch, 0));
    }
}
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 12	- Dizi Ters Çevirme

## SORU :question:
### Kendisine parametre olarak gelen  diziyi ters çeviriren recursive fonksiyonu yazınız.
```java
import java.util.Random;
public class Main {
    static String temp = "";
    public static String reverse_array(int[] arr, int i) {
        if (i == arr.length) {
            return temp;
        } else {
            temp += arr[arr.length-1-i] + " ";
            return reverse_array(arr, i+1);
        }
    }
    public static void main(String[] args) {
        Random r = new Random();
        int[] arr = new int[5];
        for (int i = 0; i < arr.length; i++) {
            arr[i]=r.nextInt(100)+1;
        }
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i]+" ");
        }
        System.out.println();
        System.out.println(reverse_array(arr, 0));
    }
}
```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# :open_book: PRATİK 13	- Kelime Ters Yazma 

## SORU :question:
### Kendisine parametre olarak gelen stringi ters çeviren recursive fonksiyonu yazınız.
```java
public class Main {
    static String temp = "";
    public static String reverse_String(String str, int i) {
        if (i == str.length()) {
            return temp;
        } else {
            temp += str.charAt(str.length()-1-i);
            return reverse_String(str, i+1);
        }
    }
    public static void main(String[] args) {
        String str = "Merhaba";
        System.out.println(str);
        System.out.println(reverse_String(str, 0));
    }
}
```
