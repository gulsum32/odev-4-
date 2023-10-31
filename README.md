# odev-4-
gulsum 20200805072


                                                                                            SORU 1
Unit test kodunuzun her bir bileşeninin beklendiği gibi çalışıp çalışmadığını test etmeyi içerir. Kodunuzun her bir yöntemini izole eder ve üzerinde testler gerçekleştirir. Birim testleri, yazılımınızın piyasaya sürülmeden önce beklendiği gibi çalıştığından emin olmanıza yardımcı olur. Unit test üç aşamadan oluşur: planlama, test senaryolarının yazılması ve birim testinin kendisinin gerçekleştirilmesi. İlk adımda geliştiriciler veya QA uzmanları birim testini hazırlar ve inceler. Bir sonraki adımda test senaryoları ve senaryolar yazarlar. Üçüncü adımda kod test edilir.

Test odaklı geliştirme, geliştiricilerin öncelikle başarısız olan birim testleri yazmasını gerektirir. Daha sonra kodu yazarlar ve test geçinceye kadar uygulamayı yeniden düzenlerler. TDD genellikle açık ve öngörülebilir bir kod tabanıyla sonuçlanır.
TÜRLERİ :
 JUnit
 JMockit
 Jtest
 TestNG
 Quilt
 NUnit
 EMMA
 Embunit
 PHPUnit
 Mocha
 Cantata
 SimpleTest

 
 Unit test amaçlanan yazılım davranışını gerçekleştirdiğini doğrulamak ve doğrulamak için ayrı kod birimlerini kullanmanıza olanak tanır. Birim testi çözümleri kod güvenliğini, güvenilirliğini ve kalitesini sağlamaya yardımcı olur. Bunlar genellikle platformlar, ana bilgisayarlar, sanal ortamlar veya donanım ortamları genelinde kod kalitesini doğrulamak için birim test senaryolarını hızlı bir şekilde oluşturan ve otomatik olarak oluşturan otomatikleştirilmiş araçlardır.


                                                                                            SORU 2

Tasarım deseni, yazılım tasarımında sık karşılaşılan sorunlara genel, yeniden kullanılabilir bir çözüm sağlar. Desen tipik olarak sınıflar veya nesneler arasındaki ilişkileri ve etkileşimleri gösterir.  Buradaki fikir, iyi test edilmiş, kanıtlanmış geliştirme/tasarım paradigmaları sağlayarak geliştirme sürecini hızlandırmaktır. 

3 tipi vardır
3 tür tasarım deseni vardır: Yaratıcı. Yapısal. Davranışsal.(Creational. Structural. Behavioral)

1. Yaratıcı Tasarım Kalıpları
Yaratıcı bir tasarım kalıbı, belirli bir durum için hangi nesnelerin oluşturulduğu konusunda rehberlik sağlayarak nesne oluşturma ve başlatma ile ilgilenir. Bu tasarım kalıpları, esnekliği artırmak ve mevcut kodu yeniden kullanmak için kullanılır.

Factory Yöntemi: Ortak bir arayüze sahip nesneler oluşturur ve bir sınıfın somutlaştırmayı alt sınıflara ertelemesine izin verir.

Abstract Factory: İlgili nesnelerden oluşan bir aile oluşturur.

Oluşturucu: Karmaşık nesneler oluşturmak, yapıyı ve temsili ayırmak için adım adım bir modeldir.

Prototip: Kod sınıflara bağımlı hale gelmeden mevcut nesnelerin kopyalanmasını destekler.

Singleton: Bir sınıf için nesne oluşturmayı yalnızca bir örnekle sınırlar.

2. Yapısal Tasarım Kalıpları
Yapısal bir tasarım kalıbı, sınıf ve nesne kompozisyonu veya nesnelerin ve sınıfların daha büyük yapılara nasıl monte edileceği ile ilgilenir.

Bağdaştırıcı: Uyumsuz arabirimlerin birlikte çalışmasına izin vermek için bir arabirimin başka bir mevcut sınıfın arabirimine nasıl değiştirileceği veya uyarlanacağı ile ilgilidir.

Köprü: Bir arabirimi uygulamasından ayırma yöntemidir.

Bileşik: Tek bir nesne olarak manipülasyonu desteklemek için bir ağaç yapısından yararlanır.

Dekoratör: İşlevselliği dinamik olarak genişletir (ekler veya geçersiz kılar).

Cephe: Büyük bir kod gövdesinin kullanımını basitleştirmek için üst düzey bir arabirim tanımlar.

Flyweight: Verileri benzer nesnelerle paylaşarak bellek kullanımını en aza indirir.

Proxy: Erişim kontrolünü etkinleştirmek, maliyeti ve karmaşıklığı azaltmak için bir nesneyi başka bir nesneyle nasıl temsil etmeniz gerektiği ile ilgilidir.

3. Davranışsal Tasarım Kalıpları
Davranışsal bir tasarım kalıbı, nesneler arasındaki iletişim ve nesneler arasında sorumlulukların nasıl atandığı ile ilgilidir.

Sorumluluk Zinciri: İşleme nesneleri zincirine devredilecek komutlar için bir yöntemdir.

Komut: Bir nesnede bir komut isteğini kapsüller.

Tercüman: Bir uygulama içinde dil öğelerinin kullanımını destekler.

Yineleyici: Koleksiyon öğelerine yinelemeli (sıralı) erişimi destekler.

Arabulucu: Sınıflar arasındaki basit iletişimi ifade eder.

Memento: Bir nesnenin dahili/orijinal durumunu kaydetme ve geri yükleme işlemidir.

Gözlemci: Diğer nesne(ler)deki değişikliklerin nesnelere nasıl bildirileceğini tanımlar.

Durum: Aşaması değiştiğinde bir nesnenin davranışı nasıl değiştirilir?

Strateji: Bir sınıf içindeki bir algoritmayı kapsüller.

Ziyaretçi: Sınıfta değişiklik yapmadan sınıf üzerinde yeni bir işlem tanımlar.

Şablon Yöntemi: Alt sınıfların belirli adımları iyileştirmesine izin verirken bir işlemin iskeletini tanımlar.

                                                                                           SORU 3
                                                                                           

import javax.swing.JOptionPane;
public class Sifre {

        public static void main(String[] args) {
            String password = "";
            boolean validPassword = false;
            while (!validPassword) {
                password = JOptionPane.showInputDialog(null, "En az 8 karakterden oluşan, en fazla 95 karakterli, en az bir harf ve en az bir sayı içeren ve hiçbir özel karakter içermeyen bir şifre girin.");
                if (password.length() < 8 || password.length() > 95) {
                    JOptionPane.showMessageDialog(null, "Şifre 8 ila 95 karakter arasında olmalıdır.");
                } else if (!password.matches(".*[a-zA-Z].*")) {
                    JOptionPane.showMessageDialog(null, "Şifre en az bir harf içermelidir.");
                } else if (!password.matches(".*\\d.*")) {
                    JOptionPane.showMessageDialog(null, "Şifre en az bir sayı içermelidir.");
                } else if (password.matches(".*[^a-zA-Z0-9].*")) {
                    JOptionPane.showMessageDialog(null, "Şifre özel karakter içeremez.");
                } else {
                    validPassword = true;
                }
            }
            JOptionPane.showMessageDialog(null, "Şifreniz: " + password);
        }
    }


                                                                                           SORU 4

public class eHesaplama {
    public static void main(String[] args) {
        double e = 1.0;
        double factorial = 1.0;
        int n = 1;
        while (n <= 20) {
            factorial *= n;
            e += 1.0 / factorial;
            n++;
        }
        System.out.println("e = " + e);
    }
}

                                                                                          SORU 2 (ÖDEVDE 2 YAZDIĞI İÇİN 2 İLE NUMARALANDIRIYORUM TEKRAR)
                                                                                          

public class eHesaplama {
    public static void main(String[] args) {
        double e = 1.0;
        double factorial = 1.0;
        int n = 1;
        while (n <= 20) {
            factorial *= n;
            e += 1.0 / factorial;
            n++;
        }
        System.out.println("e = " + e);
    }
}


                                                                                          SORU 3
 import java.util.Scanner;
public class xy {



        public static void main(String[] args) {
            Scanner input = new Scanner(System.in);
            System.out.print("İlk sayıyı girin: ");
            int sayi1 = input.nextInt();
            System.out.print("İkinci sayıyı girin: ");
            int sayi2 = input.nextInt();
            if (areFriends(sayi1, sayi2)) {
                System.out.println(sayi1 + " ve " + sayi2 + " arkadaş sayılardır.");
            } else {
                System.out.println(sayi1 + " ve " + sayi2 + " arkadaş sayılar değildir.");
            }
        }

        public static boolean areFriends(int sayi1, int sayi2) {
            int toplam1 = 0, toplam2 = 0;
            for (int i = 1; i <= sayi1 / 2; i++) {
                if (sayi1 % i == 0) {
                    toplam1 += i;
                }
            }
            for (int j = 1; j <= sayi2 / 2; j++) {
                if (sayi2 % j == 0) {
                    toplam2 += j;
                }
            }
            return toplam1 == sayi2 && toplam2 == sayi1;
        }
    }


                                                                                          SORU 4
  A)

  public class mukemmelsayi {
    public static void main(String[] args) {
        int sayi = 30;
        if (isPerfect(sayi)) {
            System.out.println(sayi + " mükemmel bir sayıdır.");
        } else {
            System.out.println(sayi + " mükemmel bir sayı değildir.");
        }
    }

    public static boolean isPerfect(int sayi) {
        int toplam = 0;
        for (int i = 1; i < sayi; i++) {
            if (sayi % i == 0) {
                toplam += i;
            }
        }
        return toplam == sayi;
    }
}


 B)

 public class mukemmelsayi2 {
    public static void main(String[] args) {
        int number;
        for (number = 1000; number < 10000; number++) {
            if (isPerfect(number)) {
                System.out.println("4 basamaklı mükemmel sayı: " + number);
            }
        }
    }

    public static boolean isPerfect(int number) {
        int sum = 0;
        for (int i = 1; i <= number / 2; i++) {
            if (number % i == 0) {
                sum += i;
            }
        }
        return sum == number;
    }
}
























































































































































