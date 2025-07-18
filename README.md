
# BANVIT SATIS ANALIZ RAPORU
Bu projede 2019 ve 2020 yillarina ait Banvit markasina ait satislar analiz edilmis olup, sonuclar farkli perspektiflerden ele alinmistir.

Bu rapor 4 sayfadan olusmaktadir:

  **1**: Giris

  **2**: Ozet

  **3**: Musteri Perspektifi

  **4**: Kategori Perspektifi


## Icindekiler
- Problem
- Veri Kaynağı
- Veri Dönüşümü
- Veri Modelleme
- Görselleştirme
- Analiz Sonuclari

### Problem

1- Toplam Satış Adeti , Toplam Ciro, Toplam Müşteri Sayısı, Toplam Sipariş Sayısı , Hafta sonu-hafta içi satış sayisi, Saatlik Satış, Müşteri başına ciro, Müşteri başına satis adeti, Ortalama sipariş tutarı nedir?

2- Kadin ve erkek musteri sayisi nedir?

3- Yas grubuna gore satislar.

4- Toplam Cironun kategorilere gore dagilimi (Sehir ve yas grubu kriterlerine gore dagilimi).


### Veri Kaynağı
Bu analiz için “Data Files” yazan dosyadaki veri setleri kullanilmistir.


### Veri Dönüşümü
Power Query'de veri temizliği ve dönüşümü yapıldı.
- Dosya isimleri Turkce karsiliklari ile degistirildi.
- Tum dosyalarda Veri Turu eslestirmesi yapildi.  
- Kullanicilar dosyasinda:
    - Isimler Ad ve Soyad olmak uzere 2 farkli sutuna ayrildi. 
    - Cinsiyet bilgisi "K" olanlar "KADIN, "E" olanlar "ERKEK" olarak yeni sutun olusturuldu. 
    - Kullanicilarin yasina gore daha sonra analizlerde kullanilmak uzere "Yas Grubu" sutunu olusturuldu.
    - DATEDIFF fonksiyonu ile kullanici yaslari hesaplandi.
- Siparis dosyasinda Hafta Turu ve Saat Araligi bilgileri eklendi.
- Urunler dosyasinda kategori basliklari degistirilip, Yeni Ana Kategori sutunu eklendi.
- Analizlerde kullanilmak uzere DAX formulleri yazildi.




### Veri Modelleme
![Model](https://raw.githubusercontent.com/burcinalim/2.Final-Projesi/refs/heads/main/Model.png?token=GHSAT0AAAAAADFOVYUODPLYB5LKEGILB2IQ2D2B2OA)


### Görselleştirme

 1- Giris Sayfasi:
 ![Giris](https://raw.githubusercontent.com/burcinalim/2.Final-Projesi/refs/heads/main/Screenshots/Giris%20Sayfasi.png?token=GHSAT0AAAAAADFOVYUOEX55XJOTAM5XJD4O2D2B33A)

 2- Ozet Sayfasi:
![Ozet](https://raw.githubusercontent.com/burcinalim/2.Final-Projesi/refs/heads/main/Screenshots/Ozet%20Sayfasi.png?token=GHSAT0AAAAAADFOVYUOW3EHHQ7K4U62FRWO2D2B4HA)

 3- Musteri Perspektifi:
![Musteri Perspektifi](https://raw.githubusercontent.com/burcinalim/2.Final-Projesi/refs/heads/main/Screenshots/Musteri%20Perspektifi.png?token=GHSAT0AAAAAADFOVYUOX3FVQGGXEQAHNWCW2D2B4KA)

4- Kategori Perspektifi:
![Kategori Perspektifi](https://raw.githubusercontent.com/burcinalim/2.Final-Projesi/refs/heads/main/Screenshots/Kategori%20Perspektifi.png?token=GHSAT0AAAAAADFOVYUOXRZQ32BAC7W3RC5I2D2B4MA)   


### Analiz Sonuclari
- Banvit Markasinin Toplam Cirosu 1.43bn ₺, Musteri Basina Dusen Ciro 1.75M ₺, Ortalama Siparis Tutari 1.68M ₺ olmustur.
- Toplam Siparis Sayisi 855 olup bu siparislerde 4689 adet urun satisi olmustur.
- Toplam 820 musteriye satis yapilmsitir. Musterilerin 461'i kadin, 359'u erkektir.
- 55+ yas grubundaki(Yasli) satis miktari en fazladir.
- En cok satis yapilan saatler 08:00-15:59 arasindadir.
- En fazla satis hafta ici yapilmistir.
- Marmara Bolgesindeki satis en fazla olurken, en az satis Dogu Anadolu Bolgesinde olmustur.
- Toplam Ciro sirasiyla Kumes, Et ve Gida kategorilerinden saglanmistir.



