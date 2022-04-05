
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




