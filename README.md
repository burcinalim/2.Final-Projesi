
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

4- Toplam Cironun kategorilere gore dagilimi (ayria sehir ve yas grubu kriterlerine gore dagilimi).


### Veri Kaynağı
Bu analiz için kullanılan veri setleri “Data Files” yazan dosya icindedir.


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
![Model]([https://github.com/burcinalim/My-Data-Analysis-Portfolio/blob/main/01-Bank%20Loan%20Analysis%20Project/Screenshots/Model%20View.png?raw=true](https://github.com/burcinalim/2.Final-Projesi/blob/main/Model.png?raw=true))


### Görselleştirme

 1- Giris Sayfasi:
 ![Giris]([https://github.com/burcinalim/My-Data-Analysis-Portfolio/blob/main/01-Bank%20Loan%20Analysis%20Project/Screenshots/1-Summary%20Page.png?raw=true](https://github.com/burcinalim/2.Final-Projesi/blob/main/Screenshots/Giris%20Sayfasi.png))

 2- Ozet Sayfasi:
![Ozet]([https://github.com/burcinalim/My-Data-Analysis-Portfolio/blob/main/01-Bank%20Loan%20Analysis%20Project/Screenshots/2-Overview%20Page.png?raw=true](https://github.com/burcinalim/2.Final-Projesi/blob/main/Screenshots/Ozet%20Sayfasi.png))

 3- Musteri Perspektifi:
![Musteri Perspektifi]([https://github.com/burcinalim/My-Data-Analysis-Portfolio/blob/main/01-Bank%20Loan%20Analysis%20Project/Screenshots/3-Details%20Page.png?raw=true](https://github.com/burcinalim/2.Final-Projesi/blob/main/Screenshots/Musteri%20Perspektifi.png?raw=true))

4- Kategori Perspektifi:
![Kategori Perspektifi]([https://github.com/burcinalim/My-Data-Analysis-Portfolio/blob/main/01-Bank%20Loan%20Analysis%20Project/Screenshots/3-Details%20Page.png?raw=true](https://github.com/burcinalim/2.Final-Projesi/blob/main/Screenshots/Kategori%20Perspektifi.png?raw=true))   


### Analiz Sonuclari
- Banvit Markasinin Toplam Cirosu 1.43bn ₺, Musteri Basina Dusen Ciro 1.75M ₺, Ortalama Siparis Tutari 1.68M ₺ olmustur.
- Toplam Siparis Sayisi 855 olup bu siparislerde 4689 adet urun satisi olmustur.
- Toplam 820 musteriye satis yapilmsitir. Musterilerin 461'i kadin, 359'u erkektir.
- 55+ yas grubundaki(Yasli) satis miktari en fazladir.
- En cok satis yapilan saatler 08:00-15:59 arasindadir.
- En fazla satis hafta ici yapilmistir.
- Marmara Bolgesindeki satis en fazla olurken, en az satis Dogu Anadolu Bolgesinde olmustur.
- Toplam Ciro sirasiyla Kumes, Et ve Gida kategorilerinden saglanmistir.



