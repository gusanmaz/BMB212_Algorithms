# NKÜ Bilgisayar Mühendisliği BMB212 Veri Yapıları Uygulama Notları ve Ödevleri

Bu repo'da uygulama derslerine ait materyallere (ders notlari, odev bilgileri, proje bilgileri, duyurular vb.) ulasabilirsiniz. 

## 1. Uygulama (22 Mart 2022)

### Instructor

Ars. Gor. Guvenc Usanmaz

Oda: B207

Bolum: Bilgisayar Muhendisligi

Email: gusanmaz <att< nku nokta edu nokta tr

### Prerequisites / Ders Hazirlik

1. [Github](https://github.com/) hesabi acilacak
2. [Repl.it](https://replit.com/) hesabi acilacak
3. [Bilgilendirme Formu](https://forms.gle/8AzYpckY7S43QTjM8) doldurulacak
4. Universite email hesaplari duzenli kontrol edilecek
5. Bu [repo](https://github.com/gusanmaz/NKU_DS_Course_2022) duzenli kontrol edilecek. Yeni odev ve proje duyurulari buradan ve/veya email yoluyla yapilacak

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

### Github Ders Sayfasi

* Ders Sayfasi: [https://classroom.github.com/classrooms/81414932-data_structures_2122_spring](https://classroom.github.com/classrooms/81414932-data_structures_2122_spring)

#### Bu haftaki alistirma linkleri

* [Min2](https://classroom.github.com/a/zrZcp24R) Program parametre olarak 2 tamsayi (integer) deger okuyup bu degerlerden kucuk olanini ekrana yazdiracak. ***Son gonderim tarihi: 25 Mayis 23:00***

``` bash
javac Main.java #Program Derleme
java Main 4 5 #Derlenmis programi 4 ve 5 argumanlari ile calistirma
4 #Program Ciktisi
java Main 9 8 #Derlenmis programi 9 ve 8 argumanlari ile calistirma
9 #Program Ciktisi
```

* [Min3](https://classroom.github.com/a/sdi4a0Zb) Program parametre olarak 3 tamsayi (integer) deger okuyup bu degerlerden kucuk olanini ekrana yazdiracak. ***Son gonderim tarihi: 25 Mayis 23:00***

``` bash
javac Main.java #Program Derleme
java Main 4 5 3 #Derlenmis programi 4, 5 ve 3 argumanlari ile calistirma
3 #Program Ciktisi
java Main 9 8 1 #Derlenmis programi 9,8 ve 1 argumanlari ile calistirma
1 #Program Ciktisi
java Main 9 -4 1 #Derlenmis programi 9,-4 ve 1 argumanlari ile calistirma
-4 #Program Ciktisi
```

* [Odev3_Faktoriyel](https://classroom.github.com/a/IWMvyac9) Program argumani olarak pozitif bir tamsayi alip, alinan bu sayinin faktoriyelini donduren bir program yaziniz. ***Son gonderim tarihi: 25 Mayis 23:00***

``` bash
javac Main.java #Program Derleme
java Main 5 #Derlenmis programi 5 degeri ile calistirma
120 #Program Ciktisi
java Main 1 #Derlenmis programi 1 degeri ile calistirma
1 #Program Ciktisi
java Main 0 #Derlenmis programi 0 degeri ile calistirma
1 #Program Ciktisi
java Main 1 #Derlenmis programi 6 degeri ile calistirma
120 #Program Ciktisi
```



