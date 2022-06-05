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

### Proje 5

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 5 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p5_results.html)

* Tum testler 20 puan degerindedir.

Bu projeyi degerlendirilmek icin hazirlanan `Main.java` dosyasinin kaynak kodlarini asagida gorebilirsiniz. Projeniz derlenmesi icin projenizdeki
`Main.java` dosyasinin icerigi asagidaki `Main.java` dosyasinin icerigi ile degistirilmistir. Not tablosundaki test numaralari uzerindeki test komutlarini
ve asagidaki `Main.java` dosyasinin icerigini inceleyerek gonderdiginiz kodlarin hangi testlere tabii tutuldugunu gorebilirsiniz.

```java
import java.lang.reflect.Method;

public class Main {
    public static void main(String args[]) throws Exception{
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
        if ((testNo < 1) || (testNo > 5)) {
            return;
        }

        Method m = Main.class.getMethod(testName, null);
        System.out.print(m.invoke(Main.class));
    }

    public static String test1(){
        HTMLNode body = new HTMLNode("body");
        HTMLNode html = new HTMLNode("html");

        HTMLNode p = new HTMLNode("p");
        HTMLNode h1 = new HTMLNode("h1");
        HTMLNode div = new HTMLNode("div");

        HTMLNode article = new HTMLNode("article");

        HTMLNode[] divChildren = new HTMLNode[]{article};
        HTMLNode[] bodyChildren = new HTMLNode[]{div, p, h1};
        HTMLNode[] htmlChildren = new HTMLNode[]{body};

        html.setChildren(htmlChildren);
        body.setChildren(bodyChildren);
        div.setChildren(divChildren);

        HTMLTree tr = new HTMLTree(html);
        return tr.GetHTML();
    }

    public static String test2(){
        HTMLNode article = new HTMLNode("article");
        HTMLNode a = new HTMLNode("a");
        HTMLNode p = new HTMLNode("p");
        HTMLNode h1 = new HTMLNode("h1");

        HTMLNode div1 = new HTMLNode("div");
        HTMLNode div2 = new HTMLNode("div");
        HTMLNode div3 = new HTMLNode("div");

        HTMLNode ol   = new HTMLNode("ol");
        HTMLNode li1   = new HTMLNode("li");
        HTMLNode li2   = new HTMLNode("li");
        HTMLNode li3   = new HTMLNode("li");
        HTMLNode li4   = new HTMLNode("li");

        HTMLNode body = new HTMLNode("body");
        HTMLNode head = new HTMLNode("head");
        HTMLNode title = new HTMLNode("title");
        HTMLNode meta = new HTMLNode("meta");
        HTMLNode html = new HTMLNode("html");

        HTMLNode[] htmlChildren = new HTMLNode[]{head, body};
        HTMLNode[] bodyChildren = new HTMLNode[]{h1, div1, article, div2};
        HTMLNode[] headChildren = new HTMLNode[]{meta, title};

        HTMLNode[] div1Children = new HTMLNode[]{div3};
        HTMLNode[] div3Children = new HTMLNode[]{p};
        HTMLNode[] pChildren = new HTMLNode[]{a};

        HTMLNode[] div2Children = new HTMLNode[]{ol};
        HTMLNode[] olChildren = new HTMLNode[]{li1, li2, li3, li4};

        html.setChildren(htmlChildren);
        body.setChildren(bodyChildren);
        head.setChildren(headChildren);

        div1.setChildren(div1Children);
        div3.setChildren(div3Children);
        p.setChildren(pChildren);

        div2.setChildren(div2Children);
        ol.setChildren(olChildren);

        HTMLTree tr = new HTMLTree(html);
        return tr.GetHTML();
    }

    public static String test3(){
        HTMLNode html = new HTMLNode("html");
        HTMLTree tr = new HTMLTree(html);
        return tr.GetHTML();
    }

    public static String test4(){
        HTMLTree tr = new HTMLTree(null);
        return tr.GetHTML();
    }

    public static String test5(){
        HTMLNode article = new HTMLNode("article");
        HTMLNode a = new HTMLNode("a");
        HTMLNode p = new HTMLNode("p");
        HTMLNode h1 = new HTMLNode("h1");


        HTMLNode div1 = new HTMLNode("div");
        HTMLNode div2 = new HTMLNode("div");
        HTMLNode div3 = new HTMLNode("div");
        HTMLNode div4 = new HTMLNode("div");

        HTMLNode ol   = new HTMLNode("ol");
        HTMLNode li1   = new HTMLNode("li");
        HTMLNode li2   = new HTMLNode("li");
        HTMLNode li3   = new HTMLNode("li");
        HTMLNode li4   = new HTMLNode("li");

        HTMLNode body = new HTMLNode("body");
        HTMLNode head = new HTMLNode("head");
        HTMLNode title = new HTMLNode("title");
        HTMLNode meta = new HTMLNode("meta");
        HTMLNode html = new HTMLNode("html");

        HTMLNode span = new HTMLNode("span");

        HTMLNode[] htmlChildren = new HTMLNode[]{head, body};
        HTMLNode[] bodyChildren = new HTMLNode[]{h1, div1, article, div2};
        HTMLNode[] headChildren = new HTMLNode[]{meta, title};

        HTMLNode[] div1Children = new HTMLNode[]{div3};
        HTMLNode[] div3Children = new HTMLNode[]{p};
        HTMLNode[] pChildren = new HTMLNode[]{a};

        HTMLNode[] div2Children = new HTMLNode[]{ol};
        HTMLNode[] olChildren = new HTMLNode[]{li1, li2, li3, li4};

        HTMLNode[] li2Children = new HTMLNode[]{span};
        HTMLNode[] h1Children = new HTMLNode[]{div4};


        html.setChildren(htmlChildren);
        body.setChildren(bodyChildren);
        head.setChildren(headChildren);

        div1.setChildren(div1Children);
        div3.setChildren(div3Children);
        p.setChildren(pChildren);

        div2.setChildren(div2Children);
        ol.setChildren(olChildren);

        li2.setChildren(li2Children);
        h1.setChildren(h1Children);

        HTMLTree tr = new HTMLTree(html);
        return tr.GetHTML();
    }

}
```

#### Cozum

Projede istenilenleri gerceklestiren `HTMLTree.java`

```java
public class HTMLTree {
    private HTMLNode root;

    public HTMLTree(HTMLNode root){
        this.root = root;
    }

    public HTMLTree(){
        this(null);
    }

    public String GetHTML(HTMLNode node, int level){
        if (node == null){
            return "";
        }
        String space = "   ";
        String levelSpace = space.repeat(level);
        String begin = levelSpace +  "<" + node.getTag() + ">\n";
        String end   = levelSpace + "</" + node.getTag() + ">\n";

        String mid = "";
        HTMLNode[] children = node.getChildren();
        if (children != null){
            for (int i = 0; i < children.length; i++){
                mid += GetHTML(children[i], level + 1);
            }
        }
        return begin + mid + end;
    }

    public String GetHTML(){
        return GetHTML(root, 0);
    }

}
```

### Proje 6

**Gonderdiginiz kodu Github kullanici adinizi tikladiginizda acilan pop-up penceresi icinde gorebilirsiniz.**

* [Proje 6 Not Tablosu](https://gusanmaz.github.io/BMB212_Algorithms/p6_results.html)

* 15 puanlik testler: Test1, Test2, Test4 ve Test4
* 10 puanlik testler: Test5, Test6, Test7 ve Test8
* 25 puanlik bonus test: Test9 **Bu testte kaynak koddaki aciklamalarin tamaminin okunup okunmadigi test edilmistir**

Bu projeyi degerlendirilmek icin hazirlanan `Main.java` dosyasinin kaynak kodlarini asagida gorebilirsiniz. Projeniz derlenmesi icin projenizdeki
`Main.java` dosyasinin icerigi asagidaki `Main.java` dosyasinin icerigi ile degistirilmistir. Not tablosundaki test numaralari uzerindeki test komutlarini
ve asagidaki `Main.java` dosyasinin icerigini inceleyerek gonderdiginiz kodlarin hangi testlere tabii tutuldugunu gorebilirsiniz.

```java
import java.lang.reflect.Method;

public class Main {
    public static Student[] generateStudents(){
        Student bugs = new Student(602, "Bugs", "Bunny", 1.09);
        Student daffy = new Student(200, "Daffy", "Duck", 2.56);
        Student mickey = new Student(150, "Mickey", "Mouse", 3.45);
        Student roadrunner = new Student(400, "Road", "Runner", 3.09);
        Student coyote = new Student(250, "Wile", "Coyote", 2.35);
        Student sam = new Student(242, "Yosemite", "Sam", 2.65);
        Student elmer = new Student(305, "Elmer", "Fudd", 0.98);
        Student tweety = new Student(406, "Tweety", "Bird", 0.95);
        Student foghorn = new Student(104, "Foghorn", "Leghorn", 1.27);
        Student tom = new Student(901, "Sylvester", "Cat", 0.50);
        Student jerry = new Student(875, "Jerry", "Mice", 3.14);

        Student[] students = new Student[]{bugs, daffy, mickey, roadrunner, coyote, sam, elmer, tweety, foghorn, tom, jerry};
        return students;
    }

    public static void main(String args[]) throws Exception {
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
        if ((testNo < 1) || (testNo > 9)) {
            return;
        }

        Method m = Main.class.getMethod(testName, null);
        m.invoke(Main.class);
    }

    public static void test1(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "ID");
        tree1.insert(students);
        String content = tree1.toDot(rootNode, "");
        System.out.println(content);
    }

    public static void test2(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "name");
        tree1.insert(students);
        String content = tree1.toDot(rootNode, "");
        System.out.println(content);
    }

    public static void test3(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "surname");
        tree1.insert(students);
        String content = tree1.toDot(rootNode, "");
        System.out.println(content);
    }

    public static void test4(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "GPA");
        tree1.insert(students);
        String content = tree1.toDot(rootNode, "");
        System.out.println(content);
    }

    public static void test5(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "ID");
        tree1.insert(students);
        tree1.printOrderedStudentsTable();
    }

    public static void test6(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "name");
        tree1.insert(students);
        tree1.printOrderedStudentsTable();
    }

    public static void test7(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "surname");
        tree1.insert(students);
        tree1.printOrderedStudentsTable();
    }

    public static void test8(){
        Student[] students = generateStudents();
        Student marvin = new Student(500, "Marvin", "Martian", 2.59);
        BSTNode rootNode = new BSTNode(marvin);
        BST tree1 = new BST(rootNode, "GPA");
        tree1.insert(students);
        tree1.printOrderedStudentsTable();
    }

    public static void test9(){
        BST tree1 = new BST();
        System.out.print(tree1.bonus());
    }
}
```
#### Cozum

Projede istenilenleri gerceklestiren `BST.java`

```java
import java.io.PrintWriter;

public class BST {
    private BSTNode root;
    private String keyType;
    private static int counter = 0;
    private static int ind;

    public BST(BSTNode node, String keyType){
        root = node;
        this.keyType = keyType;
    }

    public BST(String keyType){
        this(null,keyType);
    }

    public BST(){
        this(null, "ID");
    }

    public int Len(){
        return Len(root);
    }

    public int len(BSTNode node){
        if (node == null){
            return 0;
        }
        return len(node.left) + 1 + len(node.right);
    }

    // Bu metod agacta saklanan ogrencileri agacta kullanilan anahtar degerini gore
    // Student dizisi olarak dondurur. Bu metodu yazmak icin gerek duyarsaniz bu sinif
    // icinde yeni metodlar, fonksiyonlar ve sinif degisikenleri tanimlayabilirsiniz ama
    // mevcut sinif metodlari ve degiskenleri uzerinde bir degisiklik yapmayiniz.
    // Eger ikili arama agaciniz anahtar degeri GPA (not ortalamasi) ise bu metodun
    // dondurecegin dizinin ilk elemanindaki ogrenci not ortalamasi en dusuk son elemanindaki
    // ogrenci not ortalamasi en yuksek ogrenci olmalidir. Bir baska deyisle dondurulen
    // dizideki elemanlar anahtar degerine gore kucukten buyuge sirali olmalidir.

    // Bu metod bir altta tanimlanan PrintOrderedStudentsTable metodu tarafindan kullanilmaktadir.

    public Student[] getOrderedStudents(){
        ind = 0;
        Student[] s = new Student[len()];
        Inorder(root, s);
        return s;
    }

    // Bu metod agactaki ogrencilere ait bilgileri tablo olarak ekrana yazdirmaktadir.
    // Tablodaki ogrenciler agacta anahtar olarak belirlenen niteligi gore sirali
    // olarak yazdirilmaktadir. Ornegin ikili arama agaciniz anahtari ID (ogrenci numarasi)
    // olarak belirlendiyse bu metodu kullanarak agacinizdaki ogrencileri tablo olarak ekrana
    // yazdirmak isterseniz tablonun en ust satirinda ogrenci numarasi en kucuk ogrencinin; tablonun
    // en alt satirinda ise ogrenci numarasi en buyuk ogrencinin bilgilerini goreceksiniz.

    public void printOrderedStudentsTable(){
        System.out.format("%-15s%-15s%-12s%-4s\n", "Name", "Surname", "ID", "GPA");
        Student[] students = getOrderedStudents();
        for (Student s: students){
            System.out.format("%-15s%-15s%-12d%.2f\n",
                    s.getName(), s.getSurname(), s.getID(), s.getGPA());
        }
        System.out.println();
    }

    private void inorder(BSTNode node, Student[] s){
        if (node == null){
            return;
        }
        inorder(node.left, s);
        s[ind] = node.data;
        ind++;
        inorder(node.right, s);
    }

    // Bu metod agaci gorsellestirmek icin kullanmaktadir.
    // Metod icindeki kodlari incelemeniz tavsiye edilir ama zorunlu degildir.

    public void toDotFile(String filepath) throws Exception{
        String allRules = toDot(root, "");
        String dotFileContent = "strict digraph BST{\n\tnodesep=1.5;\n\tranksep=0.5" + allRules + "\n}";

        PrintWriter writer = new PrintWriter(filepath, "UTF-8");
        writer.print(dotFileContent);
        writer.close();
    }

    // Bu metod agaci gorsellestirmek icin kullanmaktadir.
    // Metod icindeki kodlari incelemeniz tavsiye edilir ama zorunlu degildir.

    public String toDot(BSTNode node, String rules){
        if (node == null){
            return rules;
        }

        if ((node.left == null) && (node.right != null)){
            counter++;
            String newRulePrefix = "\tnull" + counter + " [shape=point];\n";
            String newRule = "\t" + node.data.toDotString() + " -> " + "null" + counter + ";";
            rules = rules + "\n" + newRulePrefix + newRule;
        }

        if (node.left != null){
            String newRule = "\t" + node.data.toDotString() + " -> " + node.left.data.toDotString() + ";";
            rules = rules + "\n" + newRule;
        }
        if (node.right != null){
            String newRule = "\t" + node.data.toDotString() + " -> " + node.right.data.toDotString() + ";";
            rules = rules + "\n" + newRule;
        }

        if ((node.right == null) && (node.left != null)){
            counter++;
            String newRulePrefix = "\tnull" + counter + " [shape=point];\n";
            String newRule = "\t" + node.data.toDotString() + " -> " + "null" + counter + ";";
            rules = rules + "\n" + newRulePrefix + newRule;
        }

        String leftRules  = toDot(node.left, "");
        String rightRules = toDot(node.right, "");
        rules = rules + leftRules + rightRules;
        return rules;
    }


    public BSTNode insert(Student[] students){
        BSTNode ret = null;
        for (Student s : students){
            ret = insert(s);
        }
        return ret;
    }

    // Insert metodu ikili arama agacina anahtar olarak belirlenen veriye
    // gore agaca yeni eleman yerlestirmektedir.

    public BSTNode insert(Student s){
        if (keyType == "name"){
            return insertNameOrdered(s);
        }
        if (keyType == "surname"){
            return insertSurnameOrdered(s);
        }
        if (keyType == "GPA"){
            return insertGPAOrdered(s);
        }
        return insertIDOrdered(s);
    }
    
    // Bu metod agacin anahtar olarak ogrenci ismi secilmesi durumunda kullanilacaktir.
    // Bu metod kullanilarak ikili arama agacina eklenen bir ogrenci agaca ogrenci ismi
    // baz alinarak eklenecektir. Bu metodu yazabilmek icin String kutuphanesinin compareTo
    // metodunu kullanmaniz gerekmektedir.

    public BSTNode insertNameOrdered(Student s){
        BSTNode newNode = new BSTNode(s);
        if (root == null){
            root = newNode;
            return root;
        }

        BSTNode p = null;
        BSTNode n = root;

        while (n != null){

            if (n.data.getName().compareTo(s.getName()) < 0){
                p = n;
                n = n.right;
            }
            else{
                p = n;
                n = n.left;
            }
        }

        if (p.data.getName().compareTo(s.getName()) < 0){
            p.right = newNode;
        }
        else{
            p.left = newNode;
        }
        return root;
    }

    // Bu metod agacin anahtar olarak ogrenci soyismi secilmesi durumunda kullanilacaktir.
    // Bu metod kullanilarak ikili arama agacina eklenen bir ogrenci agaca ogrenci soyismi
    // baz alinarak eklenecektir. Bu metodu yazabilmek icin String kutuphanesinin compareTo
    // metodunu kullanmaniz gerekmektedir.

    public BSTNode insertSurnameOrdered(Student s){
        BSTNode newNode = new BSTNode(s);
        if (root == null){
            root = newNode;
            return root;
        }

        BSTNode p = null;
        BSTNode n = root;

        while (n != null){

            if (n.data.getSurname().compareTo(s.getSurname()) < 0){
                p = n;
                n = n.right;
            }
            else{
                p = n;
                n = n.left;
            }
        }

        if (p.data.getSurname().compareTo(s.getSurname()) < 0){
            p.right = newNode;
        }
        else{
            p.left = newNode;
        }
        return root;
    }

    // Bu metod agacin anahtar olarak ogrenci not ortalamasi (GPA) secilmesi durumunda kullanilacaktir.
    // Bu metod kullanilarak ikili arama agacina eklenen bir ogrenci agaca ogrenci not ortalamasi
    // baz alinarak eklenecektir.

    public BSTNode insertGPAOrdered(Student s){
        BSTNode newNode = new BSTNode(s);
        if (root == null){
            root = newNode;
            return root;
        }

        BSTNode p = null;
        BSTNode n = root;

        while (n != null){
            if (n.data.getGPA() < s.getGPA()){
                p = n;
                n = n.right;
            }
            else{
                p = n;
                n = n.left;
            }
        }

        if (p.data.getGPA() < s.getGPA()){
            p.right = newNode;
        }
        else{
            p.left = newNode;
        }
        return root;
    }

    // Bu metod agacin anahtar olarak ogrenci not numarasi (ID) secilmesi durumunda kullanilacaktir.
    // Bu metod kullanilarak ikili arama agacina eklenen bir ogrenci agaca ogrenci numarasi
    // baz alinarak eklenecektir.

    public BSTNode insertIDOrdered(Student s){
        BSTNode newNode = new BSTNode(s);
        if (root == null){
            root = newNode;
            return root;
        }

        BSTNode p = null;
        BSTNode n = root;

        while (n != null){
            if (n.data.getID() < s.getID()){
                p = n;
                n = n.right;
            }
            else{
                p = n;
                n = n.left;
            }
        }

        if (p.data.getID() < s.getID()){
            p.right = newNode;
        }
        else{
            p.left = newNode;
        }
        return root;
    }

    public String bonus(){
        return "futurama";
    }
    
}
```
