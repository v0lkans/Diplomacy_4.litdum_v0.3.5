# [Diplomacy 4.litdum](https://forums.taleworlds.com/index.php?topic=356425.0) Unofficial Update 

##### Bu güncelleme, modül sistemi olmadan yapılmıştır.
Yaptığım birçok değişikliğin amacı, oyundaki dengesizliğin ve adaletsizliğin biraz olsun düzelmesini sağlamaktır.

Yapay Zekâ lordlar yattığı yerden para kazanıp üstüne bir de oyuncunun ulaşamayacağı sayılarda asker ile ordu kurarken benim *emekçi, Kalradya'ya mutlak adaleti, huzuru, refahı* getirecek yegâne savaşçılarından olan kardeşlerimin bu denli zorluklar altında bırakılması büyük bir haksızlıktır.

*Bu güncelleme, Kalradya'ya adaleti getirecek savaşçılar için yapılmış bir '**Adalet**' güncellemesidir.*


- - - -
### İçerik
  * [Yapım Süreci](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5/blob/master/README.md#yapım-süreci)
  * [Değişiklikler](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5/blob/master/README.md#değişiklikler)
  * [Türkçe dili hata düzeltme güncellemesi](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5/blob/master/README.md#türkçe-dili-hata-düzeltme-güncellemesi)
  
  
- - - -
### Yapım süreci
_Modül sistemiyle çok basit ve hızlı bir şekilde yapılabilecek bu özellikleri -en önemlilerini- modül sistemi olmadan yapmak çok emek ve çok teknik bilgi isteyen bir işlem. txt dosyalarının içeriğindeki düzensiz ve anlamsız gibi görünen karmaşık sayıların ne anlama geldiğini anlamak, bu sayıları ayıklayıp, doğru olanları bulup, doğru yere, doğru sırayla yerleştirmek, yeri geldiğinde bu sayıları hexadecimal değerlere dönüştürüp, çıkan sonuca göre txt dosyalarına yeni eklemeler yapmak, hexadecimal olan değeri tekrar decimal değere döndürerek bu değere göre değişiklikler ve eklemeler yapmak günler süren bir iş. Bu bağlamda yapılan iş her ne kadar basit görünürse görünsün, benim haftalarımı aldı._

# Değişiklikler

## Oyuncu Parti büyüklüğü
###### Sadece NPC lordlarında olan özellikler artık oyuncu için de geçerli.
Oyuncu parti büyüklüğü bileşenleri karşılaştırması:

v0.3                      | Bonus         |   |  v0.3.5                   | Bonus         |
------------              | ------------- |---| -------------             | ------------- |
Taban Büyüklük            | +30           |   | Taban Büyüklük            | +30           |
Nam                       | Nam/25        |   | Nam                       | Nam/25        |
Liderlik Puanı Başına     | +1            |   | Liderlik Puanı Başına     | +1            |
Karizma Puanı Başına      | +1            |   | Karizma Puanı Başına      | +1            |
Ø                         |               |   | Sahip Olunan Kale Başına  | +20           |
Ø                         |               |   | Mareşal Olma              | +20           |
Ø                         |               |   | Kral Olma                 | +100          |
Ø                         |               |   | Seviye¹                   | formül        |

¹Seviye formülü: **Parti büyüklüğü** x ((*Oyuncunun Seviyesi* + **80** ) / **80**)
(En son bu formül uygulanır.)



- - - -
## Derebeyi Unvanları
  * ###### Derebeyi unvanları ismin sonuna da eklenebilir oldu.
  * #### Unvan değiştirme ekranındaki kutucuklar işaretlenerek unvanın isim sonuna gelmesi sağlanabilir.
  <details>
    <summary>DİKKAT! | ÇOK ÖNEMLİ! | KESİN OKUMALISIN!</summary>
    <p>Doğru çalışması için metin kutusunda değişiklik yapılması gerekmektedir.</p>
    <p>Bu ne demek? (Senaryo 1'i aç)</p>
    <details>
      <summary>Senaryo 1</summary>
      <p>1) Unvan değiştirme ekranını açtın.</p>
      <p>2) Metin kutusunu sildin ve 'Paşa' yazdın.</p>
      <p>3) Onay kutusunu da tikledin ve tamam dedin.</p>
      <p>4) Yazdığın unvanın doğru bir şekilde derebeylerinin isminin sonuna eklendiğini gördün çünkü metin kutusunda bir değişiklin yapmıştın.</p>
     <p>Sıra Senaryo 2'de.</p>
    </details>
 
 <details>
      <summary>Senaryo 2</summary>
      <p>1) Daha önceden metin kutusuna 'Paşa' yazmıştın ama onay kutusunu tiklemeyi unutmuştun ve unvan, derebeylerinin isminin başına eklenmişti.</p>
      <p>2) Unvan değiştirme ekranını tekrar açtın.</p>
      <p>3) Sadece onay kutusunu işaretleyip tamam dedin.</p>
      <p>4) Ancak unvan yine ismin başına eklendi, sonuna değil.</p>
      <p>5) Çünkü metin kutusunda herhangi bir değişik yapmadın.</p>
      <p>6) Değişiklikten kasıt şunlardır:</p>
      <p>     * Metin kutusunda yazan kelimeyi silip baştan yazmak</p>
      <p>     * Metin kutusunda yazan kelimenin son harfini silip tekrar yazmak</p>
      <p>Gibi değişiklikler.</p>
    </details>
  </details>


  ###### Bunu yapmam, modül sistemi olmadığı için yaklaşık 4 gün sürdü D: oyunun txt dosyalarını anlamak ve düzenlemek çok karmaşık ve zor bir iş.


- - - -
## Sancak Değiştirme
  * ##### Sancak taşıma hakkı kazandıktan sonra, istediğin zaman sancağını yenileyebilirsin. (Kamp Menüsü >> Sancağını Yenile)


- - - -
## Kuşatmalarda Envantere Erişebilme
  * ##### Kuşatmalarda envantere erişebilirsin.


- - - -
## Oyun Kavramları Sayfası İç Siyaset Bilgileri
  * Diplomasi modunun özelliklerinden biri olan iç siyaset değişikliklerinin detaylı açıklamaları **Oyun Kavramları** sayfasına eklendi. 


- - - -
## Kira Gelirleri
 #### Kiralardan Gelen Gelir Böleni:
  * **Oyuncu için** *~~120~~* --> *60*
  * **NPC'ler için** *~~120~~* --> *240* 
  ###### (*Oyuncu, sahip olduğu topraklardan 2 kat daha fazla kira geliri elde eder*)
  ###### (*NPC'ler, sahip oldukları topraklardan 2 kat daha az kira geliri elde eder*)


- - - -
## İşletme Ücretleri
  * *İşletme açma fiyatları* **1.2x**
  * *İşçi ve diğer masrafları* **2x**
  * *Üretim için gereken mal sayısı* **3x**
  * *Üretilen mal sayısı* **3x**
##### Arttı


- - - -
## Değirmen Refah Bonusu
* *Değirmen tek seferlik **+5** yerine her hafta **+3** refah kazandırır.*


- - - -
## Parti Morali
#### Liderlik Puanı Başına Parti Morali:
  * **Kral değilken** : *~~12~~* --> *30*
  * **Kral iken**     : *~~15~~* --> *60*


- - - -
## Haftalık Kaybedilen Nam Böleni
  * *~~200~~* --> *400*

###### (Formül = Nam / 400)
###### (**Örnek**: 2000 / 400 = 5)
###### (2000 namınız varsa her hafta 5 nam kaybedersiniz.)
###### Bu değişiklik ile haftalık kaybedilen nam 2 kat azalır.


- - - -
## Çeşitli Değişiklikler
  * NPC Parti Büyüklüğü:
    * Taban Büyüklük *~~+10~~* --> *+30*

  * *Esir yönetimi:
    * *Puan başına* **~~+5~~** --> **+10**
    #
  * *Yemek her* **~~14~~** --> **12** *saatte bir yenir.*
  #
  * Esir yakalama görevini reddetme
    * *İlişki* ~~**1 azalır**~~ --> **değişmez** 
    #
  * *Köylere ve Şehirlere girince refah seviyesi sayı olarak yazar*
  #
  * *Raporlar sekmesinde "Sonraki ödeme günü" bilgisi*
  #
  * *Gemi ücreti* **~~60000~~** --> **8000**
  #
  * Gezgin Kadın Verdiği Moral **~~4~~** --> **40**
  #
  * Askerlere bira ısmarlama
    * Birim fiyatı **~~25~~** --> **5**
    * Verdiği moral **~~1~~** --> **5**
    #
  * Askerlere şarap ısmarlama
    * Birim fiyatı **~~50~~** --> **10** 
    * Verdiği moral **~~2~~** --> **10**
  
  #
  * Ok sayıları 40 arttırıldı.

# Türkçe dili hata düzeltme güncellemesi
Oyunda karşılaştığım yazım hatalarını, çeviri hatalarını, hatalı gösterimleri elimden geldiğince düzeltmeye çalıştım.

Aynı zamanda bazı gösterimlerin daha anlaşılabilir olması için eklemeler de yaptım.

Hatalar büyük oranda giderildi, ancak hâlâ, karşılaşmadığım ya da gözümden kaçmış hatalar olabilir.
