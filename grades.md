# Ödev Notlandırmaları

## Bilgilendirme

* **Gonderdiginiz kodu  Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**
* Her test icin calistirilan komutlari imleci ilgili testin altina getirerek gorebilirsiniz.
* Her test icin kodunuzun nasil cikti urettigini ve uretmesi gereken ciktiyi imleci sizle ilgili satirdaki test hucrelerine getirerek gorebilirsiniz.
* Ayni sekilde kodunuz derlenmesini icin calistirilan komutun ciktisini imleci sizle ilgili satirdaki Compilation hucresine getirerek gorebilirsiniz.
* Notlar sonraki odev ve projelerde daha farkli bir formatta aciklanirsa bunla ilgili ayri aciklama yapilacaktir. 

## Ilk 3 Odev Degerlendirmesi Hakkinda Bilgilendirme

* Sadece otomatik testleri gececek sekilde yazilmis kodlar tespit edildiginden kodlarinizi test etmek icin yeni testler yazilmistir. 
* Derlenebilen kodlara 20 puan verilmistir.
* Ilk 2 odevde 20 farkli test uygulanmistir. Her testin toplam puana 4 puan katkisi vardir.
* Ucuncu odevde 10 farkli test uygulanmistir. Her testin toplam puana 8 puan katkisi vardir.
* Odev gonderen arkadaslara tesekkurler :)
* Odevlerden tam puan alamayan arkadaslar lutfen odevlerden tam puan alan arkadaslarin kodlari ile kendi kodlarini karsilastirsin odev not tablolari uzerinden.

## Odev Not Tablolari 

### Odev1, Odev2 ve Odev3

* [Ödev 1 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw1_results.html)
* [Ödev 2 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw2_results.html)
* [Ödev 3 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw3_results.html)

### Odev4, Odev5 ve Odev6

**Gonderdiginiz kodu  Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Ödev 4 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw4_results.html)
* [Ödev 5 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw5_results.html)
* [Ödev 6 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/hw6_results.html)

Bu odevlerin degerlendirilmesinde kullanilan metin dosyalari asagida verilmistir.

* list1.txt: `       `
* list2.txt: `8      `
* list3.txt: `0      `
* list4.txt: `-9 4 5 4 543 32 1`
* list5.txt: `5 6`
* list6.txt: `8 99 -999 90 13 2`
* list7.txt: `10    56  67 90 90`
* list8.txt: `89 30 12 14 16   88`
* list9.txt: `88   888  888 8`
* list10.txt `12345 907`

### Proje 1

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 1 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/p1_results.html)

### Proje 2

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 2 Not Tablosu](https://gusanmaz.github.io/NKU_DS_Course_2022/p2_results.html)

Bu projeyi degerlendirilmek icin hazirlanan `Main.java` dosyasinin kaynak kodlarini asagida gorebilirsiniz. Projeniz derlenmesi icin projenizdeki
`Main.java` dosyasinin icerigi asagidaki `Main.java` dosyasinin icerigi ile degistirilmistir. Not tablosundaki test numaralari uzerindeki test komutlarini
ve asagidaki `Main.java` dosyasinin icerigini inceleyerek gonderdiginiz kodlarin hangi testlere tabii tutuldugunu gorebilirsiniz.

* `Main.java`

```java
import java.lang.reflect.InvocationTargetException;
import java.lang.reflect.Method;

public class Main {

    public static void Test1(){
        LinkedList list = new LinkedList();
        list.Append(5);
        list.Append(6);
        list.Append(2);
        list.Append(6);
        System.out.println(list.Sum());
    }

    public static void Test2(){
        LinkedList list = new LinkedList();
        list.Append(456);
        System.out.println(list.Sum());
    }

    public static void Test3(){
        LinkedList list = new LinkedList();
        list.Append(1);
        list.Append(64);
        list.Append(25);
        list.Append(64);
        list.Append(53);
        list.Append(62);
        list.Append(211);
        list.Append(-98);
        System.out.println(list.Sum());
    }

    public static void Test4(){
        int[] num1 = {1,6,7,9,14,100};
        LinkedList a = new LinkedList(num1);
        System.out.println(a.IsSorted());
    }

    public static void Test5(){
        int[] num1 = {10, 9, 8, 7};
        LinkedList a = new LinkedList(num1);
        System.out.println(a.IsSorted());
    }

    public static void Test6(){
        int[] num1 = {-100, -50, 0, 79, 799, 1235};
        LinkedList a = new LinkedList(num1);
        System.out.println(a.IsSorted());
    }

    public static void Test7(){
        int[] num1 = {100};
        LinkedList a = new LinkedList(num1);
        System.out.println(a.IsSorted());
    }

    public static void Test8(){
        int[] num1 = {};
        LinkedList a = new LinkedList(num1);
        System.out.println(a.IsSorted());
    }

    public static void Test9(){
        int[] num1 = {1,6,7,9,14};
        int[] num2 = {-1, 4,8,10,11,15,19};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test10(){
        int[] num1 = {1,3,6};
        int[] num2 = {2,4};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test11(){
        int[] num1 = {5,5,6};
        int[] num2 = {2,4,4};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test12(){
        int[] num1 = {};
        int[] num2 = {2,4,9};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test13(){
        int[] num1 = {};
        int[] num2 = {2};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test14(){
        int[] num1 = {};
        int[] num2 = {2};
        LinkedList a = new LinkedList(num1);
        LinkedList b = new LinkedList(num2);
        LinkedList c = LinkedList.MergeSortedLists(a,b);
        c.Print();
    }

    public static void Test15(){
        LinkedList list = new LinkedList();
        list.Append(1);
        list.Append(64);
        list.Append(25);
        list.Append(64);
        list.Append(53);
        list.Append(62);
        list.Append(211);
        list.Append(-98);
        list.PrintReverse();
    }

    public static void Test16(){
        LinkedList list = new LinkedList();
        list.Append(5);
        list.Append(6);
        list.Append(2);
        list.Append(6);
        list.PrintReverse();
    }

    public static void Test17(){
        LinkedList list = new LinkedList();
        list.Append(5);
        list.PrintReverse();
    }


    public static void main(String[] args) throws Exception {
        String testName = args[0];
        if (!testName.contains("Test")){
            return;
        }
        String testNoStr = testName.replaceAll("Test", "");
        int testNo = -1;
        try{
            testNo = Integer.parseInt(testNoStr);
        }
        catch (Exception ex){
            return;
        }
        if ((testNo < 1) || (testNo > 17)) {
            return;
        }

        Method m = Main.class.getMethod(testName, null);
        m.invoke(Main.class);
    }
}



