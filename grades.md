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

* [Ödev 1 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw1_results.html)
* [Ödev 2 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw2_results.html)
* [Ödev 3 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw3_results.html)

### Odev4, Odev5 ve Odev6

**Gonderdiginiz kodu  Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* Uygulanan her test 10 puan degerindedir.

* [Ödev 4 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw4_results.html)
* [Ödev 5 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw5_results.html)
* [Ödev 6 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/hw6_results.html)

Bu odevlerin degerlendirilmesinde kullanilan metin dosyalari asagida verilmistir.

* list1.txt:  `       `
* list2.txt: `8      `
* list3.txt: `0      `
* list4.txt: `-9 4 5 4 543 32 1`
* list5.txt: `5 6`
* list6.txt: `8 99 -999 90 13 2`
* list7.txt: `10    56  67 90 90`
* list8.txt: `89 30 12 14 16   88`
* list9.txt: `88   888  888 8`
* list10.txt: `12345 907`

### Proje 1

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 1 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p1_results.html)

* Son 2 test (Test 41, Test 42) 10 puan diger testler 2 puan degerindedir.

* Test islemini kolaylastirmak adina C# kodlari kodun anlaminda bir degisiklik yapilmadan Java koduna cevrilmis ve testler bu ceviri kodlar uzerinde uygulanmistir. Odeve ait PDF dokumaninda String fonksiyonlari kullanilmamasi istenmistir. C#'da bu String metodlari kullanilarak kodlanan metodlar degerlendirmeye alinmamistir.

### Proje 2

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 2 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p2_results.html)

* Ilk 3 test (Test 1, Test 2, Test 3) 10 puan diger testler 5 puan degerindedir.

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
```

### Proje 3

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 3 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p3_results.html)

* Tum testler 10 puan degerindedir.

### Proje 4

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 4 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p4_results.html)

* Tum testler 5 puan degerindedir.

Bu projeyi degerlendirilmek icin hazirlanan `Main.java` dosyasinin kaynak kodlarini asagida gorebilirsiniz. Projeniz derlenmesi icin projenizdeki
`Main.java` dosyasinin icerigi asagidaki `Main.java` dosyasinin icerigi ile degistirilmistir. Not tablosundaki test numaralari uzerindeki test komutlarini
ve asagidaki `Main.java` dosyasinin icerigini inceleyerek gonderdiginiz kodlarin hangi testlere tabii tutuldugunu gorebilirsiniz.

```java
import java.lang.reflect.Method;

public class Main {
    public static int[] values1 = new int[]{4};
    public static int[] values2 = new int[]{4, 7};
    public static int[] values3 = new int[]{9,65, 43, 12, 34, 90, 456, 907, 101, -89, 45, -90};
    public static int[] values4 = new int[]{3, 4, 5, 6, 9, 1, 0, 80, 800, -80, 45, 9000, 98765, 123456, -999};
    public static int[] values5 = new int[]{2, 1, 3};
    public static int[] values6 = new int[]{10, 6, 8, 4, 15, 12, 11, 7};
    public static int[] values7 = new int[]{1, 5, 0, -4, 9, 8, 3, 10};
    public static int[] values8 = new int[]{60, 25, 40, 56, 55, 43, 67, 90, 85, 10};
    public static int[] values9 = new int[]{1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    public static int[] values10 = new int[]{9, 8, 7, 6, 5, 1, 19, 20, 25, 18, 17, 21};

    public static void insertList(BST tree, int[] arr){
        for (int value: arr){
            tree.Add(value);
        }
    }

    public static void breakBST(BST tree, int oldValue, int newValue){
        TreeNode n = tree.root;
        while (n != null) {
            if (n.val == oldValue){
                n.val = newValue;
                return;
            }

            if (n.val < oldValue){
                n = n.right;
            }

            if (n.val > oldValue){
                n = n.left;
            }
        }
        return;
    }

    public static void test1(){
        BST t = new BST();
        insertList(t, values1);
        t.PrintPreOrder();
    }

    public static void test2(){
        BST t = new BST();
        insertList(t, values2);
        t.PrintPostOrder();
    }

    public static void test3(){
        BST t = new BST();
        insertList(t, values3);
        t.PrintPreOrder();
    }

    public static void test4(){
        BST t = new BST();
        insertList(t, values4);
        t.PrintPostOrder();
    }

    public static void test5(){
        BST t = new BST();
        insertList(t, values5);
        t.PrintPreOrder();
    }

    public static void test6(){
        BST t = new BST();
        insertList(t, values6);
        t.PrintPostOrder();
    }

    public static void test7(){
        BST t = new BST();
        insertList(t, values7);
        t.PrintPreOrder();
    }

    public static void test8(){
        BST t = new BST();
        insertList(t, values8);
        t.PrintPostOrder();
    }

    public static void test9(){
        BST t = new BST();
        insertList(t, values9);
        t.PrintPreOrder();
    }

    public static void test10(){
        BST t = new BST();
        insertList(t, values10);
        t.PrintPostOrder();
    }

    public static void test11(){
        BST t = new BST();
        insertList(t, values1);
        System.out.println(t.IsBST());
    }

    public static void test12(){
        BST t = new BST();
        insertList(t, values2);
        System.out.println(t.IsBST());
    }

    public static void test13(){
        BST t = new BST();
        insertList(t, values3);
        System.out.println(t.IsBST());
    }

    public static void test14(){
        BST t = new BST();
        insertList(t, values4);
        System.out.println(t.IsBST());
    }

    public static void test15(){
        BST t = new BST();
        insertList(t, values5);
        System.out.println(t.IsBST());
    }

    public static void test16(){
        BST t = new BST();
        insertList(t, values6);
        breakBST(t, 10, 100);
        System.out.println(t.IsBST());
    }

    public static void test17(){
        BST t = new BST();
        insertList(t, values7);
        breakBST(t, -4, 2);
        System.out.println(t.IsBST());
    }

    public static void test18(){
        BST t = new BST();
        insertList(t, values8);
        breakBST(t, 67, 59);
        System.out.println(t.IsBST());
    }

    public static void test19(){
        BST t = new BST();
        insertList(t, values9);
        breakBST(t, 5, -5);
        System.out.println(t.IsBST());
    }

    public static void test20(){
        BST t = new BST();
        insertList(t, values10);
        breakBST(t, 6, 12);
        System.out.println(t.IsBST());
    }


    public static void main(String[] args) throws Exception {
        String testName = args[0];
        if (!testName.contains("test")) {
            return;
        }
        String testNoStr = testName.replaceAll("test", "");
        int testNo = -1;
        try {
            testNo = Integer.parseInt(testNoStr);
        } catch (Exception ex) {
            return;
        }
        if ((testNo < 1) || (testNo > 20)) {
            return;
        }

        Method m = Main.class.getMethod(testName, null);
        m.invoke(Main.class);
    }

}
```




