
# Proje 1

* Proje aciklamalarina [bu baglantidaki PDF'den](https://raw.githubusercontent.com/gusanmaz/OOP_CSharp_Alistirmalari/master/Programlama_temelleri.pdf) ulasabilirsiniz.
* PDF'de sadece ***2  Fonksiyon Aciklamalari*** aciklamalari kismini okumaniz yeterlidir.
* Projeyi Java veya C# kullanarak kodlayabilirsiniz.
* Son proje gonderme tarihi: ***3 Nisan 2022 23:59'dur***. Lutfen bu tarihten sonra odev icin size tahsis edilen repo'da bir degisiklik (commit) yapmayiniz.
* Projeler bireysel yapilacaktir. Kopya tespiti durumununda kopya odevlere 0 verilecektir.Ayrica kopya odevler icin idari islem yapilabilir. 
* Bu dokumani gunluk olarak takip etmeniz tavsiye edilir. Proje ile ilgili yapilabilecek degisiklikler, duyurular, duzeltmeler bu dokumanda ve/veya email yoluyla bildirilecektir.


[**Proje Davet Linki**](https://classroom.github.com/a/rzlSOwsh)

* Projeyi Java ile kodlayacaksaniz sadece Main.java dosyasi uzerinde
* Proje C# ile kodlayacaksaniz sadece Main.cs dosyasi uzerinde
degisiklikler yapiniz.

* Java ile kodlama yaptiysaniz repo'daki Main.cs dosyasini; C# ile kodlama yaptiysaniz repo'daki Main.java dosyasini silebilirsiniz.
* Derleme hatasi veren projeler degerlendirmeye alinmayacaktir, bu projeler 0 olarak notlandirilacaktir.
* Projenizindeki fonksiyonlarin calisma zamani hatasi (runtime error) uretmedigine emin olun. Bu tur hatalar da projeden dusuk not, hatta 0 almaniza neden olabilir.

* :warning::exclamation: **Fonksiyon iclerinde I/O (kullanicidan veri okuma/ekrana deger yazdirma) islemi yapmayiniz.**

# Duzeltmeler

* PDF'deki `Ornegin KatalanSayisi(10) ifadesi 4862 degerinidondurecektir.` ifadesinin `Ornegin KatalanSayisi(9) ifadesi 4862 degerinidondurecektir.` seklinde degistirilmesi gerekmektedir.
* :warning::exclamation: PDF dokumaninda ToplaPalindrome6 metodunun donus degeri turu **int** olarak verilmistir. Bu metodun donus degeri **long** olarak degistirilmelidir.

# Proje 2

Proje 2 [Davet Linki](https://classroom.github.com/a/qDWDSkJQ)

## Proje Aciklamalari

* LinkedList.java dosyasindaki yorum satirlarini okuyup, ilgili metod ve fonksiyonlarda gerekli degisiklikleri yapiniz.
* Calisir hale getirmeniz gereken metod ve fonksiyonlar Sum, PrintReverse, IsSorted ve MergeSortedLists'dir.
* Yukarida ismi gecen metod ve fonksiyonlarin imzalarinda bir degisiklik yapmayiniz.
* Sablon kodda verilen diger metodlarda, fonksiyonlarda (main haric) ve constructor'larda degisiklik yapmayiniz.
* Sablon koddaki dosya isimlerinde ve sinif isimlerinde degisiklik yapmayiniz.
* Proje son gonderim tarihi **17 Nisan 2022 23:59**'dur.
* Proje iceriginde degisiklikler, eklemeler, duzeltmeler yapilabilir. Lutfen universite email hesaplarinizi, [BMB212 Github sayfasini](https://github.com/gusanmaz/NKU_DS_Course_2022) ve [Ders Github Issues sayfasini](https://github.com/gusanmaz/NKU_DS_Course_2022/issues) duzenli takip ediniz.
* Projeleriniz otomatik program tarafindan degerlendirilecektir. Gondereceginiz kodlarin derlendigine ve tam olarak projede istenilen sekilde olmasina dikkat ediniz.
* Bu proje bireysel bir projedir. Kesinlikle baskasindan aldiginiz kodlari gondermeyiniz! 

## Projenin Derlenmesi

```bash
javac *.java
```

## Projenin Calistirilmasi

Sablon dosyadaki main fonksiyonun icerigi asagidaki gibidir. 

```java
public static void main(String[] args){
        // main altinda linkedlist sinifi icin yazdiginiz metodlarin dogru
        // calisip calismadigini test edebilirsiniz.
        // main altinda yazacaginiz kodlar derleme hatasi uretmedigi surece
        // notlandirmaya olumlu veya olumsuz etkisi olmayacaktir.

        LinkedList list = new LinkedList();
        list.Append(5);
        list.Append(6);
        list.Append(2);
        list.Print();
        System.out.println(list.Sum());
        System.out.println(list.IsSorted());

        int[] num1 = {1,6,7,9,14};
        int[] num2 = {-1, 4,8,10,11,15,19};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        a.Print();
        System.out.println(a.IsSorted());
        b.Print();
        System.out.println(b.IsSorted());

        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
        System.out.println(c.IsSorted());
        System.out.println(c.Sum());
        c.PrintReverse();
    }
```

LinkedList sinifinda istenilen degisikler dogru bir sekilde yapilir ve main fonksiyonunuzun icerigi yukaridaki gibi olursa programiniz calistirdiginizda alacaginiz cikti asagidaki gibi olacaktir.

```bash
java Main
| 5 | --> | 6 | --> | 2 | --> |NULL|
13
false
| 1 | --> | 6 | --> | 7 | --> | 9 | --> | 14 | --> |NULL|
true
| -1 | --> | 4 | --> | 8 | --> | 10 | --> | 11 | --> | 15 | --> | 19 | --> |NULL|
true
| -1 | --> | 1 | --> | 4 | --> | 6 | --> | 7 | --> | 8 | --> | 9 | --> | 10 | --> | 11 | --> | 14 | --> | 15 | --> | 19 | --> |NULL|
true
103
|NULL| <-- | 19 | <-- | 15 | <-- | 14 | <-- | 11 | <-- | 10 | <-- | 9 | <-- | 8 | <-- | 7 | <-- | 6 | <-- | 4 | <-- | 1 | <-- | -1 |
```

## Sablon Proje Kodlari

Asagida bu repoda verilen sablon kodlar bulunmaktadir. Uzerinde degisiklik yaptiginiz dosyalarin ilk hallerine buradan ulasabilirsiniz.

### Node.java

```java
public class Node {
    public int value;
    public Node next;

    public Node(int v){
        value = v;
        next  = null;
    }

    public Node(){
        
    }

}
```

### LinkedList.java

```java
public class LinkedList {
    private Node head;

    public LinkedList(){
        head = null;
    }

    public LinkedList(int[] arr){
        head = null;
        for (int i = 0; i < arr.length; i++){
            Node n = new Node(arr[i]);
            Append(n);
        }
    }

    public void Append(int val){
        Node newNode = new Node();
        newNode.value = val;
        newNode.next  = null;
        // Yukaridaki 3 satirlik ifade yerine asagidaki yoruma cevrilmis ifade yazilabilirdi.
        // Node newNode = new Node(val); 

        if (head == null){
            head = newNode;
            return;
        }

        Node n = head;
        while (n.next != null){
            n = n.next;
        }
        n.next = newNode;
    }

    public void Append(Node newNode){
        if (head == null){
            head = newNode;
            return;
        }

        Node n = head;
        while (n.next != null){
            n = n.next;
        }
        n.next = newNode;
    }

    public void Print(){
        Node n = head;
        while (n != null){
            System.out.print("| " + n.value + " |" + " --> ");
            n = n.next;
        }
        System.out.println("|NULL|");
    }

    // Bu metod bagli listenin elemanlarini sondan basa dogru sirali okarak ekrana yazdirir.
    // Bu metodun ciktisi Print metodununun ciktisinin yonu degistirilmis sekli olmalidir.
    // Bu metodu kodlamak icin dizi, ArrayList, String metodlari vb. kullanmayiniz.
    // Bu metodu recursive (oz yinelemeli) sekilde yazabilirsiniz. Bu metodu yazmak icin baska
    // bir metod tanimlayip PrintReverse metodu icinde tanimlamis oldugunuz bu metodu kullanabilirsiniz.

    public void PrintReverse(){
        
    }

    // Bu metod bagli listedeki elemanlarin toplamini dondurur.

    public int Sum(){
       
    }

    // IsSorted() bagli liste kucukten buyuge sirali ise true aksi durumda false dondurur.
    // Bagli liste bos ise veya tek elemanli ise IsSorted() true dondurur.

    public boolean IsSorted(){
        
    }

    // MergeSortedLists(LinkedList m, LinkedList n) parametre olarak iki tane kucukten
    // buyuge sirali bagli liste alir ve bu listelerdeki elemanlarin kucukten buyuge
    // siralandigi bir bagli liste dondurur.

    public static LinkedList MergeSortedLists(LinkedList m, LinkedList n){
        
    }
}
```

### Main.java

```java
public class Main {
    public static int[] Reverse(int[] a){
        int[] b = new int[a.length];
        for (int i = 0; i < a.length; i++){
            b[i] = a[a.length - 1 - i];
        }
        return b;
    }

    public static void main(String[] args){
        // main altinda linkedlist sinifi icin yazdiginiz metodlarin dogru
        // calisip calismadigini test edebilirsiniz.
        // main altinda yazacaginiz kodlar derleme hatasi uretmedigi surece
        // notlandirmaya olumlu veya olumsuz etkisi olmayacaktir.

        LinkedList list = new LinkedList();
        list.Append(5);
        list.Append(6);
        list.Append(2);
        list.Print();
        System.out.println(list.Sum());
        System.out.println(list.IsSorted());

        int[] num1 = {1,6,7,9,14};
        int[] num2 = {-1, 4,8,10,11,15,19};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        a.Print();
        System.out.println(a.IsSorted());
        b.Print();
        System.out.println(b.IsSorted());

        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
        System.out.println(c.IsSorted());
        System.out.println(c.Sum());
        c.PrintReverse();
    }
}

}
```

# Proje 3

* [Proje 3 Davet Linki](https://classroom.github.com/a/9wDKu0aQ)

Size hazir verilen Stack.java sinifina ait kodlar asagidaki gibidir.

```java
public class Stack {
    public char[] s;
    public int N;

    public Stack(int cap) {
        s = new char[cap];
    }

    public int size() {
        return N;
    }

    public boolean isEmpty(){
        return N == 0;
    }


    public void push(char item) {
        s[N++] = item;
    }

    public char pop() {
        return s[--N];
    }
    
    
    // Bu fonksiyon parametre olarak aldigi iki yiginin icerigi ayni ise true aksi halde false degerini dondurur.
    // Iki yiginda bos ise bu fonksiyon true degerini dondurur.
    // Iki yiginin da icerigi ayni fakat kapasiteleri farkli ise (s dizisinin eleman sayilari farkli ise) fonksiyon true degerini dondurur.
    // Fonksiyon taniminda (function signature) herhangi bir degisiklik yapmayiniz.
    
    public static boolean Equal(Stack s1, Stack s2){
        // Fonksiyon icini uygun sekilde doldurunuz.
    }
}
```

Size hazir verilen Main.java sinifina ait kodlar asagidaki gibidir.


```java
public class Main {
    public static void main(String args[]){
        // main fonksiyonun icini uygun sekilde doldurunuz.
    }
}
```

* Main icine yazilacak kod calistirildiginda komut satiri argumani olarak alinacak 2 string turde degerin birbirine esit olup olmadigi kontrol edilecektir. Program, degerler esitse true; degilse ekrana false yazdiracaktir.
* Arguman olarak verilecek stringlerde karsilasabileceginiz `%` karakteri ozel bir karakter olarak degerlendirilmelidir. Bu karakter stringdeki kendinden bir soldaki karakteri siler. Komut satiri argumanlarindaki `%` karakteri ile klavyedeki Backspace tusunun ayni islevi yerine getirdigini soyleyebiliriz.
* Main altinda Stack sinifinin sizin icin tanimlanmis metodlarini ve/veya icini doldurmaniz gereken Equal metodunu kullanmaniz gerekebilir.
* Size verilen Stack sinifinda yapmaniza izin verilen tek degisiklik Equal metodunun icinin bu metodunun istenilen islevi yerine getirecek sekilde doldurulmasidir. Stack sinifindaki diger metodlarin, yapicilarin kodu ile oynamayiniz. Sinifa yeni metod veya degisken eklemeyiniz.

### Projenin Derlenmesi

```bash
javac Main.java Stack.java
```

### Projenin Calistirilmasi

```bash
java Main nku nku
true
java Main nku nkuu
false
java Main yemek% yeme
true
java Main abc%d abd
true
java aa%% a
false
java App Apple%%
true
java ge%l go%l
true
java aa%% bb%%
true
java aa%%% dd%%
true
java %% %
true
java www www
true
java ftp http
false
```

### Ipucu

Yardimci Kod Ornegi: Asagidaki kod ornegi bir stringin karaketerlerini sirayla alt alta yazdirmaktadir. Kodun altinda kodun ciktisi da verilmistir.
Main altinda yazacaginiz kodda stringi olusturan karakterler uzerinde tek tek islem yapmak gerekebilecegi icin bu ornek kod size hazir verilmistir.

```java
public class Main {
    public static void main(String args[]){
        String s = "Bilgisayar";
        for (int i = 0; i < s.length(); i++){
            char c = s.charAt(i);
            System.out.println(c);
        }
    }
}
```

Kod Ciktisi:

```bash
B
i
l
g
i
s
a
y
a
r
```





