# Merkez Bankası Rezerv Hesaplama

1-Merkez bankası internet sitesinden öncelikle "Uluslararası Rezervler ve Döviz Likiditesi" başlığı kapsamında Veri (Haftalık) kısmından PDF indirilir.

https://www.tcmb.gov.tr/wps/wcm/connect/TR/TCMB+TR/Main+Menu/Istatistikler/Odemeler+Dengesi+ve+Ilgili+Istatistikler/Uluslararasi+Rezervler+ve+Doviz+Likiditesi/


Bu pdf den bazı bilgiler alacağız;

--Kırmızı ile işaretlediğim yerler brüt rezerv içerikleridir.

![1](https://github.com/AnlasEkonomi/MerkezBankasiRezerv/assets/173607120/8a90319e-893b-4a89-b008-ecee81ba777b)


Bu değerlerin toplamı pdf en başındaki "Resmi rezerv varlıkları" rakamını verir. Bu değer bankanın açıklanan tarih için "Brüt Rezerv" rakamıdır.

Döviz Varlıklar: 81.042

IMF: 149

SDR: 7304

Altın: 59.127

Toplam: 147.622

Şimdi brüt değerden net değere doğru gitmem gerekiyor. Sonuçta bu değer bizim elimizde olan toplam rezerv iken, bu rezervlerin içerisindeki bazı tutarlar bizim borçlarımız. Yani yükümlülüklerimiz.

--Bunlar temelde 2 ye ayrılır;

1-Swap yükümlülükleri

2-Bilançodaki yükümlülükleri

Swap yükümlülükleri yukarıdaki pdf den ulaşabileceğimiz bir bilgidir.

![2](https://github.com/AnlasEkonomi/MerkezBankasiRezerv/assets/173607120/0109cc48-2b61-4393-a6a4-844af7c9fe63)

28.691 + 3.490 = 32.181 (Bu yükümlülük olmasından dolayı gösterimi negatif değerdir)

Şimdi geldik bilanço yükümlülüğüne;

Bunun için EVDS sisteminden "Merkez Bankası Haftalık Vaziyeti" son açıklanan tarihteki haftalık bilançoya ulaşmamız lazım.

![3](https://github.com/AnlasEkonomi/MerkezBankasiRezerv/assets/173607120/54ac776b-ba25-47fe-9156-14ebaf638b4d)


Bunu indirirken bizlere gerekli olan kalemler sırası ile şu şekildedir;

P32.Bankacılık   Sektörü Mevduatı YP(Bin TL)-Düzey   

P321.Yurt İçi Bankalar YP(Bin TL)-Düzey   

P3211.Nakit YP(Bin TL)-Düzey   

P3212.Teminat YP(Bin TL)-Düzey   

P32121.Nakit YP(Bin TL)-Düzey   

P3213.Altın YP (Bin TL)-Düzey   

P323.Zorunlu Karşılıklar Bloke Hesabı   YP(Bin TL)-Düzey   

P3231.Nakit YP(Bin TL)-Düzey   

P3232.Altın YP(Bin TL)-Düzey   

P4.Yurt Dışı Bankalar YP(Bin TL)-Düzey   

P5.Rezerv Dilimi İmkanı YP(Bin TL)-Düzey   

P6.SDR Tahsisatı YP(Bin TL)-Düzey

![4](https://github.com/AnlasEkonomi/MerkezBankasiRezerv/assets/173607120/c37a4ba3-1edc-43a4-8924-afcfd6997c7d)

!!!Burada dikkat etmeniz gereken nokta, ilk baişta indirdiğimiz brüt rezerv pdf tarihi yani veri tarihi ne ise EVDS ile elde ettiğimiz bilanço verileri aynı tarih olmalıdır.

Şimdi geldik bu bilanço verilerinin yabancı para birimi cinsine çevrilmesine.

Bunun için MB açıklanan kur rakamları sayfasına gideceğiz.

https://www.tcmb.gov.tr/kurlar/kurlar_tr.html

Öncelikle bu kur sayfasında tarih girmemiz gerekiyor. Bu tarih açıklanan veri tarihinden bir gün öncesi olarak seçilmelidir. Elimizdeki veriler 21.06.2024 tarihine ait ise 20.06.2024 tarihindeki kur ekranına gitmem gerekiyor.

Bu ekranda ise "DolarTL Alış Kuru" değerini alacağız. Örneğimizde bu değer 32.5711 dir.

Bu değeri bilançodaki değerleri düzeltmek için kullanacağız. Bilançodaki değerleri bu kur değerine bölme işlemi bunu gerçekleştirir.

![vvvvv](https://github.com/AnlasEkonomi/MerkezBankasiRezerv/assets/173607120/28146e89-c352-4150-b385-d6f0ddc14b50)


Şimdi ise bilanço yükümlülüklerimizi ayrıştırmamız gerekiyor.

SDR: 7304

Rezerv Dilimi: 149

Yurt Dışı Bankalar: 21.574

Bu üçünün toplamı 29.027 bunu bir kenara yazalım

Geriye kalanlar ise dolar ve altın cinsinden ayırmamız istendiğinde ayırabileceğimiz kalemlerdir. Yurtiçi bankalar ile Zorunlu karşılıklar toplamı Bankacılık Sektör Mevduatını verir. Bu toplam 73.953 dür ve bu da bizim bilanço yükümlülüğümüzdür. 

Eğer altın ve dolar olarak ayırmak istersek de Zorunlu Karşılık içindeki altın ve döviz ayrılır daha sonra Yurt içi bankalardaki altın döviz ayrılır ve toplamı yine bankacılık sektör mevduatını verir.


Gelelim nihai hesaba;

Brüt Rezerv: 147.622

Swap Yükümlülüğü: 32.181

Bilanço Yükümlülüğü: 102.980 (29.027+73.953)

Net Rezerv (Brüt-Bilanço Yükümlülüğü): 44.642

Swap Hariç Net Rezerv: (Net Rezerv-Swap): 12.461

Saygılarımla...
