IO atau input output adalah mekanisme memasukkan suatu data kedalam program dan
bagaimana mengeluarkan hasil dari program tersebut.

Meskipun pengertian i/o secara lebih luas lebih dari hal tersebut, namun disini
kita akan menggunakan terbatas pada input dan output di terminal.

## Input

Input di Java dapat menggunakan 2 cara (yang umum digunakan).

### Scanner

```java
import java.util.Scanner;

class Main{
    public static void main(String args[]){
        Scanner scan = new Scanner(System.in);
        int i = scan.nextInt();
    }
}
```

### BufferReader

```java
import java.io.BufferedReader;
import java.io.StreamReader;

class Main{
    public static void main(String args[]){
        BufferedReader r = new BufferedReader(new StreamReader(System.in));
        int a = Integer.parseInt(b.readLine());
    }
}
```

## Output

Output di Java dapat menggunakan 2 cara (yang umum digunakan).

### System.out.print()

fungtion print() meskipun kita menuliskan kodenya dua baris namun hasil atau outputnya tidak menjadi dua baris, solusinya kita bisa menggunakan function yang kedua yaitu println() dimana dengan fungsi tersebut dapat menambahkan baris baru pada outputnya.

```java
class Main{
    public static void main(String args[]){
        System.out.println("Hello world");
        System.out.print("Hello world");
    }
}
```

### System.out.printf

```java
class Main{
    public static void main(String args[]){
        String data = "Hello world";
        System.out.printf("%s", data);
    }
}
```
