# Verilerin nasıl işleneceği hakkında ön planlama
## Daha Önceden Mezun Olunduysa, Mezun Olunan Üniversite: [x]
- drop

## Lise Bolum Diger: [x]
- drop

## Lise Adi Diger: [x]
- drop

## Girisimcilikle Ilgili Deneyiminizi Aciklayabilir misiniz?: [x]
- evet-hayır
  
## Hangi STK'nin Uyesisiniz?: [x]
- drop
  
## Uye Oldugunuz Kulubun Ismi: [x]
- evet-hayır

## Baska Kurumdan Aldigi Burs Miktari: [x]
- Cümle içindeki en büyük sayıyı al.
- tüfe verisine göre paranın değerini hesapla
- Boş ise '-'.

## Burs Aldigi Baska Kurum:
- evet-hayır

## Burslu ise Burs Yuzdesi: [x]
- Boş ise '0'.

## Daha Once Baska Bir Universiteden Mezun Olmus: [x]
- Boş ise 'Hayır'.

## Ingilizce Seviyeniz?: [x]
- drop

## Anne Sektor: [x]
- 0 - ve Boş değerlere - konacak
- anne çalışma durumuna göre diğer yapılacak

## Spor Dalindaki Rolunuz Nedir?: [x]
- '0', '-' ve 'nan' ise '-'.

## Stk Projesine Katildiniz Mi?: [x]
- Boş değerler hayır olarak yazılacak.

## Baba Sektor: [x]
- 'Anne Sektör' ile aynı

## Aktif olarak bir STK üyesi misiniz?: [x] 
- Boş değerler 'Hayır' olarak yazılacak.

## Girisimcilikle Ilgili Deneyiminiz Var Mi?: [x]
- Boş değerler 'Hayır' olarak yazılacak.

## Baba Calisma Durumu: [x]
- Baba sektor'de veri var ise çalışma durumu 'Evet' yapılacak.

## Anne Calisma Durumu: [x]
- Anne sektor'de veri var ise çalışma durumu 'Evet' yapılacak.

# Ingilizce Biliyor musunuz?: [ ]
- senelere göre knn veya boş değerlere hayır
- sorulmayan seneleri bul

## Lise Mezuniyet Notu: [x]
- 4'lük yazılanları 100'lüğe çevir.
- Boş değerlere 'Not ortalaması yok' yazılacak.

## Universite Not Ortalamasi: [x]
- 'Not ortalaması yok' yerine 'ortalama bulunmuyor' yazılacak.
- Boş değerler ve 'Hazırlığım' yazanlara 'ortalama bulunmuyor' yazılacak.

## Ikametgah Sehri: [x]
- Küçük harf yapılacak.
- ',' veya '-' veya '/' varsa bunlar ve bunlardan önce yazılan her şey silinecek.
- Boş değerler, '------' ve 'OpenAIrequestfailedtimeout' yazanlar 'Lise Sehir'ine göre belirlenecek.

## Girisimcilik Kulupleri Tarzi Bir Kulube Uye misiniz?: [x]
- Boş değerlere 'Hayır' yazılacak.

## Kardes Sayisi: [x]
- Boş değerlere '0' yazılacak.
- float şeklinde yazılanlarda '.' ve sonrasındaki sayı silinecek.
- Cümle içindeki sayısı al. (re.findall()).

## Profesyonel Bir Spor Daliyla Mesgul musunuz: [x]
- Boş değerlere 'Hayır' yazılacak.

## Lise Sehir: [x]
- Küçük harf yapılacak.
- ',' veya '-' veya '/' varsa bunlar ve bunlardan önce yazılan her şey silinecek.
- Boş değerlere 'ikametgah' yaz.
  
## Lise Bolumu: [x]
- hepsi küçük harf yapılacak.
- filtreleme

## Baba Egitim Durumu: [x]
- Küçük harf yapılacak.
- Boş değer ve '0' 'Eğitim Yok' olarak yazılacak.
  
## Lise Turu: [x]
- Hepsi küçük harf yapılacak.
- filtreleme

## Dogum Yeri: [x]
- Boş değerlere 'ikametgah' değerleri yazılacak
- '/' veya '-' varsa bun ve bundan önce yazılan her şey silinecek.
  
## Anne Egitim Durumu [x]
- Hepsi küçük harf yapılacak.
- boş değerlere eğitim yok

## Lise Adi: [x]
- drop

## Universite Kacinci Sinif: [x]
- Hepsi küçük harf yapılacak.
- 'Daha Önceden Mezun Olunduysa, Mezun Olunan Üniversite' var veya Daha Once Baska Bir Universiteden Mezun Olmus 'evet' ise 'Mezun'

## Universite Turu: [x]
- boşlar drop

## Bölüm:
- drop

## Baska Bir Kurumdan Burs Aliyor mu?: [x]
- Boş değerlere hayır

## Dogum Tarihi: [x]
- Ayın ismini yazanlarla sayıları değiştir.
- datetime'a dönüştür
- aykırı ve boş verileri temizle
- eğer kayıp fazla ise KNN veya üniversite sınıfı verilerini kullanarak doldur

## Cinsiyet: [x]
- Boş değer olanlara 'Belirtmek istemiyorum' yazılacak

## Universite Adi: [x]
- Hepsi küçük harf yapılacak.

## Degerlendirme Puani: [x]
- Boş değer olanı sil.

## Basvuru Yili: [x]
- datetime'a dönüştür

## Görselleştirme
- senelere göre sorulmamış sorular
    - sorulmayan seneler için knn
- 'Değerlendirme Puanı, yıl' tablosu
- bence test verisinde olmayan bütün veriler silinmeli ve 2016 verileri test edilmeli 'berke'
## Bütün verilere uygulanacak işlemler
- Hepsi küçük harf yapılacak.
- Aykırı değerler silinecek.
- numerik değerler float veya int tipine dönüştürülecek.