# NKÜ Bilgisayar Mühendisliği Veri Yapıları (BMB212) Dersi Uygulamalarının Not ve Duyuruları

Bu repo'da uygulama derslerine ait materyallere (ders notlari, odev bilgileri, proje bilgileri, duyurular vb.) ulasabilirsiniz. 

## 1. Uygulama (22 Mart 2022)

### Instructor

Ars. Gor. Güvenç Usanmaz

Oda: B207

Bolum: Bilgisayar Muhendisligi

Email: gusanmaz <att< nku nokta edu nokta tr

### Prerequisites / Ders Hazirlik

1. [Github](https://github.com/) hesabi acilacak
2. [Repl.it](https://replit.com/) hesabi acilacak
3. [Bilgilendirme Formu](https://forms.gle/8AzYpckY7S43QTjM8) doldurulacak
4. Universite email hesaplari duzenli kontrol edilecek
5. Bu [repo](https://github.com/gusanmaz/NKU_DS_Course_2022) duzenli kontrol edilecek. Yeni odev ve proje duyurulari buradan ve/veya email yoluyla yapilacak

### Odev ve Proje Sayfalari

* [Assignments Page - Odev Duyurulari](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/odevler.md)
* [Projects Page - Proje Duyurular](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/projeler.md)
* [Odev ve Proje Notlandirmalari](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/grades.md)

Bu sayfalari duzenli takip etmeniz gerekmektedir. Yeni odev duyurulari, yeni proje duyurulari, daha onceden verilmis proje ve odevlerle ilgili yeni bilgiler/duzeltmeler bu sayfalardan ilan edilecektir.  



### Onerilen Kaynaklar

* [CS50](https://cs50.harvard.edu/college/2022/spring/)
* [Introduction to Programming in Java](https://introcs.cs.princeton.edu/java/home/)
* [Algorithms, 4th Edition by Robert Sedgewick and Kevin Wayne](https://algs4.cs.princeton.edu/home/) 
* [Algoritmalar, Robert Sedgewick, NOBEL AKADEMİK YAYINCILIK](https://www.kitapyurdu.com/kitap/algoritmalar/498451.html)
* [Introduction to Algorithms, Fourth Edition](https://www.amazon.com/Introduction-Algorithms-fourth-Thomas-Cormen/dp/026204630X)

**Algorithm Visualisation**

* [https://visualgo.net/en](https://visualgo.net/en)
* [https://algorithm-visualizer.org/](https://algorithm-visualizer.org/)
* [https://www.cs.usfca.edu/~galles/visualization/Algorithms.html](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html)

### Git

![Git vs Renaming](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/images/git_vs_renaming.jpg)

* [Pro Git book](https://git-scm.com/book/en/v2)
* [Turkce Git 101](https://aliozgur.gitbooks.io/git101/content/)
* [Git Basit Rehber](https://rogerdudler.github.io/git-guide/index.tr.html)
* [Yeni Baslayanlar icin Git 101](https://medium.com/@muratcanbur/yeni-ba%C5%9Flayanlar-i%C3%A7in-git-101-ff7ea5b3eff9)
* [Git Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)
* [Git Github Kullanim Rehberi](https://www.enesonmez.com/git-github-nedir-kullanim-rehberi/)
* [Introduction to Git - talk by Scott Chacon](https://youtu.be/xbLVvrb2-fY)
* [Introduction to Git with Scott Chacon of GitHub](https://youtu.be/ZDR433b0HJY)
* [Git 101 | Git, GitHub nedir?](https://youtu.be/nyIdgGD74c4)
* [Git, GitHub ve GitLab Kullanımı Playlist](https://www.youtube.com/playlist?list=PLPrHLaayVkhnNstGIzQcxxnj6VYvsHBHy)

### IDE Kullanimi

* [Jet Brains](https://www.jetbrains.com/)
   *  [IntelliJ IDEA](https://www.jetbrains.com/idea/)
   *  [CLion](https://www.jetbrains.com/clion/)
   *  [PyCharm](https://www.jetbrains.com/pycharm/)
   *  [GoLand](https://www.jetbrains.com/go/)
   *  [Rider](https://www.jetbrains.com/rider/)
* [VS Code](https://code.visualstudio.com/)
* Visual Studio
* [Repl.it](https://replit.com)


### Terminal Kullanimi

* [Linux Tutorial for Beginners - Learn Linux and the Bash Command Line](https://ryanstutorials.net/linuxtutorial/)
* Windows? [Cygwin](https://www.cygwin.com/)

### Debugging - Hata Ayiklama

![Debugging Cat](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/images/debug_cats.jpeg)

* Break points
* Step into vs. Step over
* Step out
* Variable values
* [IntelliJ IDEA Debugging](https://www.jetbrains.com/help/idea/debugging-code.html)

### Command Line Arguments

* [Command Line Arguments](https://docs.oracle.com/javase/tutorial/essential/environment/cmdLineArgs.html)
* [Java Ornek Kodu - Github Gist](https://gist.github.com/gusanmaz/49dae8ffd1b1511e7c394a259dae785d) 
* [Replit Ornek Kodu](https://replit.com/@GuvencUsanmaz/CommandLineArgsJavaExample1)

![Linux CLI Power](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/images/linux_cli.jpg)

Komut satirindan alinan iki tam sayinin toplamini ekrana yazdiran kod:

```java
public class Main {
  public static void main(String args[]) {
    int num1 = Integer.parseInt(args[0]);
    int num2 = Integer.parseInt(args[1]);
    System.out.println(num1 + num2);
  }
}
```

Main.java isimli dosyada saklanabilecek yukarida verilen kodun derlenmesi icin calistirilmasi gereken terminal komutu:

```bash
javac Main.java
```

javac programinin derleme sonrasi olusturdugu calistirilabilir program Main.class'in calistirilmasi:

```bash
java Main 4 5 
```

Calistirilan programin ciktisi:

```bash
9
```

### Bu haftaki alistirma linkleri

Not: Bu haftaki derste bahsedilen otomatik kod testi problemi cozulmustur. Kodunuz 'Commit changes' butonuna tiklandiktan sonra otomatik olarak derlenip, puanlandirilabilmektedir. Gonderdiginiz kodun derlenip, derlenmedigini, derlendiyse testleri gecip gecmedigini Actions sekmesi/tabi altinda gorebilirsiniz.

* [Min2](https://classroom.github.com/a/zrZcp24R) Program parametre olarak 2 tamsayi (integer) deger okuyup bu degerlerden kucuk olanini ekrana yazdiracak. ***Son gonderim tarihi: 25 Mart 23:00***

``` bash
javac Main.java #Program Derleme
java Main 4 5 #Derlenmis programi 4 ve 5 argumanlari ile calistirma
4 #Program Ciktisi
java Main 9 8 #Derlenmis programi 9 ve 8 argumanlari ile calistirma
9 #Program Ciktisi
```

* [Min3](https://classroom.github.com/a/sdi4a0Zb) Program parametre olarak 3 tamsayi (integer) deger okuyup bu degerlerden kucuk olanini ekrana yazdiracak. ***Son gonderim tarihi: 25 Mart 23:00***

``` bash
javac Main.java #Program Derleme
java Main 4 5 3 #Derlenmis programi 4, 5 ve 3 argumanlari ile calistirma
3 #Program Ciktisi
java Main 9 8 1 #Derlenmis programi 9,8 ve 1 argumanlari ile calistirma
1 #Program Ciktisi
java Main 9 -4 1 #Derlenmis programi 9,-4 ve 1 argumanlari ile calistirma
-4 #Program Ciktisi
```

* [Odev3_Faktoriyel](https://classroom.github.com/a/IWMvyac9) Program argumani olarak pozitif bir tamsayi alip, alinan bu sayinin faktoriyelini donduren bir program yaziniz. ***Son gonderim tarihi: 25 Mart 23:00***

``` bash
javac Main.java #Program Derleme
java Main 5 #Derlenmis programi 5 degeri ile calistirma
120 #Program Ciktisi
java Main 1 #Derlenmis programi 1 degeri ile calistirma
1 #Program Ciktisi
java Main 0 #Derlenmis programi 0 degeri ile calistirma
1 #Program Ciktisi
java Main 3 #Derlenmis programi 6 degeri ile calistirma
6 #Program Ciktisi
```

### Metin Dosyasindaki Degerleri Diziye Aktarma

Eliminiz altinda `liste.txt' isimli bir metin dosyasi olsun ve bu dosyada tam sayilar saklansin. Tam sayilar birbirinden bosluk (space) karakteri ile ayrilsin. Ornegin liste.txt dosyamizin icerigi asagidaki gibi olabilir.

`5 6 7 8 9 4 3 5 4 3`

Bu dosyayi okuyup icerigini int turde bir diziye aktarabiliriz. Parametre olarak dosya ismi (ya da yolu) alip o dosyadaki degerleri sirasiyla iceren int dizisi donduren `ReadIntArrayFromFile` metodunu inceleyiniz. Bu metodu icinde tam sayilarin birbirlerinden bosluk karakteri ile ayrildigi turde bir metin dosyasinda kullabiliriz; ama bu fonksiyonu bu formatta olmayan bir dosyanin iceriginden dizi elde etmek icin kullanmak beklenmeyen sonuclar uretebilir. Bu  metodu bundan sonraki bazi odevlerde kullanmaniz gerekecektir. Bu nedenle metodun amacinin ne oldugunu ve metodun nasil kullanilabilecegini anlamaniz bazi odevleri kolay kodlayabilmenizde faydali olacaktir. 

```java
import java.io.FileReader;
import java.util.*;

public class Main {
    public static void main(String[] args){
        int[] elems = ReadIntArrayFromFile("list.txt");
        int i = 1;
        for (int v : elems){
            System.out.println("Dosyadaki " + i  + ". tam sayi " + v + "'dir.");
            i++;
        }
    }

    public static int[] ReadIntArrayFromFile(String path){
        List<Integer> intList = new ArrayList<Integer>();
        Scanner sc;
        try {
            sc = new Scanner(new FileReader(path)).useDelimiter("\\s+");
        }
        catch(Exception ex){
            return null;
        }

        while (sc.hasNext()) {
            String token = sc.next();
            int num = Integer.parseInt(token);
            intList.add(num);
        }

        int[] intArray = new int[intList.size()];
        int ind = 0;
        for (Integer v:intList){
            intArray[ind++] = v.intValue();
        }
        return intArray;
    }

}
```

Yukaridaki programin ciktisi:

```bash
Dosyadaki 1. tam sayi 5'dir.
Dosyadaki 2. tam sayi 6'dir.
Dosyadaki 3. tam sayi 7'dir.
Dosyadaki 4. tam sayi 8'dir.
Dosyadaki 5. tam sayi 9'dir.
Dosyadaki 6. tam sayi 4'dir.
Dosyadaki 7. tam sayi 3'dir.
Dosyadaki 8. tam sayi 5'dir.
Dosyadaki 9. tam sayi 4'dir.
Dosyadaki 10. tam sayi 3'dir.
```

Asagida bu metodu kullanan baska bir kod ve bu kodun terminal ciktisi verilmektedir. Verilen kod komut satiri argumani olarak alinan dosyadaki sayilarin toplamini ekrana yazdirmaktadir.

```java
import java.io.FileReader;
import java.util.*;

public class Main {
    public static void main(String[] args){
       int[] arr = ReadIntArrayFromFile(args[0]);
       int sum = 0;
       for (int i = 0; i < arr.length; i++){
           sum += arr[i];
       }
       System.out.println(sum);
    }

    public static int[] ReadIntArrayFromFile(String path){
        List<Integer> intList = new ArrayList<Integer>();
        Scanner sc;
        try {
            sc = new Scanner(new FileReader(path)).useDelimiter("\\s+");
        }
        catch(Exception ex){
            return null;
        }

        while (sc.hasNext()) {
            String token = sc.next();
            int num = Integer.parseInt(token);
            intList.add(num);
        }

        int[] intArray = new int[intList.size()];
        int ind = 0;
        for (Integer v:intList){
            intArray[ind++] = v.intValue();
        }
        return intArray;
    }
}
```

```bash
cat listem.txt #cat komutu ile dosya icerigini ekrana yazdirabilirsiniz
1 3 5 89 -9 87 34
javac Main.java #Yukaridaki kodu derlemek icin terminale yazdigimiz komut
java Main.class listem.txt #Derlenmis programi listem.txt argumani ile calistirma
210 #Calistirdigimiz programin ciktisi
```

### Yeni Odevler (Odev Verilme Tarihi: 28 Mart 2022)

Bu odevleri kodlayabilmeniz icin `ReadIntArrayFromFile` metodunu kullanmaniz gerekmektedir. Sablon kodlarda size hazir verilen bu metodun kodlari ile oynamayiniz ve herhangi bir degisiklik yapmayiniz!

* [Odev4 DiziCarpim](https://classroom.github.com/a/Y5yCjGxG) Arguman olarak icinde tamsayilarin saklandigi ve bu sayilarin bosluk karakteri ile birbirlerin ayrildigi bir metin dosyasinin konumunu (path, yol, dosya ismi) alan ve bu dosyadaki sayilarin carpimini ekrana yazdiran bir program yaziniz. Metin dosyasi bos bir dosya ise (icinde hic tamsayi bulunmazsa program ekrana 1 (carpma isleminin etkisiz elemani) yazdirmalidir. ***Son gonderim tarihi: 3 Nisan 2022 23:00***

```bash
cat list.txt
1 5 6 9 9 -3
javac Main.java
java Main list.txt
-7290
```

```bash
cat deneme.txt
1 1 1 -1 1 1 8 -4 9   2 2 1
javac Main.java
java Main deneme.txt
1152
```

```bash
cat deneme3.txt
     #deneme3.txt dosyasinda sadece bosluk karakterleri var. 
javac Main.java
java Main deneme3.txt
1 # 1 carpma isleminin etkisiz elemanidir.
```

* [Odev5 DiziCiftOrtalama](https://classroom.github.com/a/hpXYd1dN) Arguman olarak icinde tamsayilarin saklandigi ve bu sayilarin bosluk karakteri ile birbirlerin ayrildigi bir metin dosyasinin konumunu (path, yol, dosya ismi) alan ve bu dosyadaki sayilardan cift olanlarin ortalamasini ekrana yazdiran bir program yaziniz. Listede cift sayi yoksa ortalama 0 olacagi icin ekrana sifir yazdirilmalidir. Tam sayilarin ortalamasi rasyonel sayi (double) cikabilir. Programiniz kodlarken bu durumu goz onunde bulundurunuz! ***Son gonderim tarihi: 3 Nisan 2022 23:00***

```bash
cat a.txt
1 4 6 9 9 -3
javac Main.java
java Main a.txt
5
```



```bash
cat deneme.txt
0 0 0 0 1 1 8 -4 9 2 0 0
javac Main.java
java Main deneme.txt
0.666
```


```bash
cat cift.txt
1 6 4 4
javac Main.java
java Main cift.txt
4.666
```

* [Odev6 DiziFark](https://classroom.github.com/a/Kw0B3ymL) Arguman olarak icinde tamsayilarin saklandigi ve bu sayilarin bosluk karakteri ile birbirlerin ayrildigi bir metin dosyasinin konumunu (path, yol, dosya ismi) alan ve bu dosyadaki sayilardan en buyugu ile en kucugu arasindaki farki `max - min` ekran yazdiran bir program yaziniz. Dosyadaki en kucuk ve en buyuk sayi ayni sayi program ekrana 0 yazdirmalidir. Ayni sekilde arguman olarak alinan dosyada herhangi bir sayi bulunmuyorsa program ekrana 0 yazdirmalidir.  ***Son gonderim tarihi: 3 Nisan 2022 23:00***

```bash
cat a.txt
1 4 6 9 9 -3
javac Main.java
java Main a.txt
12 #9 - (-3)
```



```bash
cat deneme.txt
1 1 6 7 5 8 8 8 1 
javac Main.java
java Main deneme.txt
7 # 8 - 1
```


```bash
cat cift.txt
4 4 4 4 4
javac Main.java
java Main cift.txt
0 #4 - 4
```

### Vize Uygulama Sorulari ve Cozumleri

* [Gunduz Sorusu](https://gist.github.com/gusanmaz/1d113e4ce797bd9504531e3621fbef76)
* [Gunduz Cozumu](https://gist.github.com/gusanmaz/848659b167877875ed00c931e0e7fc95)
* [Gece Sorusu](https://gist.github.com/gusanmaz/b930c94bc2170bc2a78719054b6e81c2)
* [Gece Cozumu](https://gist.github.com/gusanmaz/5c2ca4dfd2e4da377dbb44ae33519b40)

### 9 Mayis 2022 (Odev ve Proje Degerlendirmeleri)

* 4., 5. ve 5. odev ile 1. 2. proje gonderimleriniz degerlendirilmistir. 
* 1., 2. ve 3. odev ile ilgili not degerlendirme tablolari guncellenmistir.
* [Notlariniz gormek icin tiklayiniz!](https://github.com/gusanmaz/NKU_DS_Course_2022/blob/main/grades.md)




