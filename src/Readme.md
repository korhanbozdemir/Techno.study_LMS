# Proje Adı: TestingProject_3 > techno.study & e-junkie.com
https://techno.study/tr/  &  https://e-junkie.com/wiki/demo/  environment’larının bazı fonksiyonlarının test edilmesi.

## Proje Açıklaması:
Bu proje, Techno Study'nin "/tr" alanının test edilmesi sürecine odaklanırken, aynı zamanda daha önce hotfix edilmiş olan E-Junkie environment'ının da bazı fonksiyonlarının test edilmesini içerir. İki ana bölümden oluşur: Birinci bölümde, Techno Study web sitesinin testi ve kullanılabilirliğinin artırılması yer alırken, ikinci bölümde ise E-Junkie environment'ının işlevselliğinin kontrol edilmesi hedeflenir.

### Proje Dosyaları
[Techno Study User Story & Test Case](https://docs.google.com/spreadsheets/d/1bj8hUQpKCPcmBBXvw10sdSty96mn-lTe/edit?usp=drive_link&ouid=108357966207576195639&rtpof=true&sd=true)

[E-Junkie User Story & Test Cases](https://docs.google.com/spreadsheets/d/1kX-Inssewg-ZS_opwR4XcXJ1GYjoaHJ9/edit?usp=drive_link&ouid=108357966207576195639&rtpof=true&sd=true)

[Screenshots](https://drive.google.com/drive/folders/1qRt0JuKU38YVHPPfabLohDIbW4kgtpGz?usp=drive_link)

## Başlarken

### Gereksinimler

Bu proje, aşağıdaki sistemler ve gereksinimler ile test edilmiştir:

- **İşletim Sistemleri:**
    - Windows 10, 11
    - macOS Big Sur
    - Ubuntu 20.04 LTS   
<br>
- **Entegre Geliştirme Ortamları (IDE):**
    - IntelliJ IDEA 2021.2
    - Eclipse 2021-06   
<br>
- **Programlama Dili:**
    - Java 8SE, 11, 20   
<br>
- **Bağımlılıklar:**
    - Selenium WebDriver 4.11.0
    - TestNG 6.14.3, 7.4.0   

### Kurulum
Proje kurulumu için aşağıdaki adımları takip edebilirsiniz:

0. IntelliJ IDEA Community Edition'ı [buradan](https://www.jetbrains.com/idea/download/) indirin ve kurun.
1. Java 8SE (JDK 1.8)'i [buradan](https://www.oracle.com/java/technologies/downloads/#java8-windows) indirin ve kurun.
   (JDK 20 de, [buradan](https://www.oracle.com/java/technologies/downloads/#java20) indirilebilir.)
2. [IntelliJ'de Maven projesi açma](https://www.jetbrains.com/help/idea/maven-support.html#create_new_maven_project) 
3. [IntelliJ'de TestNG Kullanımı](https://www.jetbrains.com/help/idea/testng.html)
4. Proje bağımlılıklarını yönetmek için Maven kullanıyorsanız, `pom.xml` dosyasını güncelleyerek gerekli bağımlılıkları ekleyin:

   ```xml
   <dependencies>
       <!-- Selenium WebDriver -->
       <dependency>
           <groupId>org.seleniumhq.selenium</groupId>
           <artifactId>selenium-java</artifactId>
           <version>4.11.0</version>
       </dependency>
   
       <!-- TestNG -->
       <dependency>
           <groupId>org.testng</groupId>
           <artifactId>testng</artifactId>
           <version>7.4.0</version>
       </dependency>

    <!-- SLF4J (Simple Logging Facade for Java) -->
    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>slf4j-nop</artifactId>
        <version>1.7.36</version>
    </dependency>

    <!-- Commons IO -->
    <dependency>
        <groupId>commons-io</groupId>
        <artifactId>commons-io</artifactId>
        <version>2.11.0</version>
    </dependency>
    
    <!-- Diğer bağımlılıklarınız -->
   
   </dependencies>

## Sürüm Geçmişi

* 0.2
    * Çeşitli hata düzeltmeleri ve optimizasyonlar
    * Commit değişiklikleri
* 0.1
    * İlk Sürüm
