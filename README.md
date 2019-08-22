# [Diplomacy 4.litdum](https://forums.taleworlds.com/index.php?topic=356425.0) Unofficial Update 

#### Birkaç yenilik ve değişiklik getiren bir güncelleme.

- - - -
### İçerik
  * [Yapım Sürecinin Zorluğu](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5#yapım-sürecinin-zorluğu)
  * [Değişiklikler](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5#değişiklikler)
  * [Türkçe dili hata düzeltme güncellemesi](https://github.com/v0lkans/Diplomacy_4.litdum_v0.3.5#türkçe-dili-hata-düzeltme-güncellemesi)
  
  
- - - -
### Yapım sürecinin Zorluğu
###### Bu güncelleme, modül sistemi olmadan yapılmıştır.
_Modül sistemiyle çok basit ve hızlı bir şekilde yapılabilecek bu özellikleri -en önemlilerini- modül sistemi olmadan yapmak çok emek ve çok teknik bilgi isteyen bir işlem. Txt dosyalarının içeriğindeki düzensiz ve anlamsız gibi görünen karmaşık sayıların ne anlama geldiğini anlamak, bu sayıları ayıklayıp, doğru olanları bulup, doğru yere, doğru sırayla yerleştirmek, yeri geldiğinde bu sayıları hexadecimal değerlere dönüştürüp çıkan sonuca göre txt dosyalarına yeni eklemeler yapmak, hexadecimal olan değeri tekrar decimal değere döndürerek bu değere göre değişiklikler ve eklemeler yapmak günler süren bir iş. Bu bağlamda yapılan iş her ne kadar basit görünürse görünsün, benim haftalarımı aldı._

# Değişiklikler

## Oyuncu Parti büyüklüğü
###### NPC lordlarında olan özellikler artık oyuncu için de geçerli.
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
Ø                         |               |   | _Seviye**¹**_             | formül**²**   |

¹Bu ayar varsayılan olarak kapalıdır. Bu ayarı da dahil etmek için oyun dosyalarındaki "**script Seviye_Carpanli.txt**" dosyasının adını "**script.txt**" olarak değiştirin. (_Varsayılan "**script.txt**" dosyasını ister silin, ister adını değiştirin. Size kalmış_)

²Seviye formülü: **Parti büyüklüğü** x ((*Oyuncunun Seviyesi* + **80** ) / **80**)
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


  ###### Bunu yapmam yaklaşık 4 gün sürdü D: Değişiklikler arasında en çok uğraştıranı da bu.


- - - -
## Sancak Değiştirme
  * ##### Sancak taşıma hakkı kazandıktan sonra, istediğin zaman sancağını yenileyebilirsin. (Kamp Menüsü >> Sancağını Yenile)


- - - -
## Kuşatmalarda Envantere Erişebilme
  * ##### Kuşatmalarda envantere erişebilirsin.


- - - -
## Kira Gelirleri
 #### Kiralardan Gelen Gelir Böleni:
  * **Oyuncu için** *120* --> **değişmedi**
  * **NPC'ler için** *120* --> *80*
  ###### (*Oyuncuya verilen avantajlar, NPC'lerin savaşlarda biraz güçsüz kalmasına neden oluyor. Bu yüzden, biraz daha para kazanmalarında sakınca yoktur diye düşünüyorum.*)



- - - -
## Değirmen Refah Bonusu
* *Değirmen tek seferlik **+5** yerine her hafta **+3** refah kazandırır.*


- - - -
## Parti Morali
#### Liderlik Puanı Başına Parti Morali:
  * **Kral değilken** : *~~12~~* --> *15*
  * **Kral iken**     : *~~15~~* --> *30*


- - - -
## Haftalık Kaybedilen Nam Böleni
  * *~~200~~* --> *400*

###### (Formül = Nam / 400)
###### (**Örnek**: 2000 / 400 = 5)
###### (2000 namınız varsa her hafta 5 nam kaybedersiniz.)
###### Bu değişiklik ile haftalık kaybedilen nam 2 kat azalır.


- - - -
## Oyun Kavramları Sayfası İç Siyaset Bilgileri
  * Diplomasi modunun özelliklerinden biri olan iç siyaset değişikliklerinin detaylı açıklamaları ben tarafından Türkçe'ye çevirildi ve **Oyun Kavramları** sayfasına eklendi. 


- - - -
## Çeşitli Değişiklikler
  * NPC Parti Büyüklüğü:
    * Taban Büyüklük *~~+10~~* --> *+30*
  #
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
  * *Gemi ücreti* **~~60000~~** --> **20000**
  #
  * Gezgin Kadın Verdiği Moral **~~4~~** --> **20**
  #
  * Askerlere bira ısmarlama
    * Birim fiyatı **~~25~~** --> **15**
    * Verdiği moral **~~1~~** --> **4**
    #
  * Askerlere şarap ısmarlama
    * Birim fiyatı **~~50~~** --> **30** 
    * Verdiği moral **~~2~~** --> **8**
  
  #
  * Normal okların ve kundaklı yay oklarının sayıları 40 arttırıldı. (Talim ve arena okları dahil değildir.)

# Türkçe dili hata düzeltme güncellemesi
Oyunda karşılaştığım yazım hatalarını, çeviri hatalarını, hatalı gösterimleri elimden geldiğince düzeltmeye çalıştım.

Aynı zamanda bazı gösterimlerin daha anlaşılabilir olması için eklemeler de yaptım.

Hatalar büyük oranda giderildi, ancak hâlâ, karşılaşmadığım ya da gözümden kaçmış hatalar olabilir.
