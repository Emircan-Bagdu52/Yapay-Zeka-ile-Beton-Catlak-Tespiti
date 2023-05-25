<h1>Beton Çatlakları</h1>
Görüntü işleme tekniklerini kullanarak beton yüzeylerdeki çatlakları otomatik olarak tespit etmektir. Bu projenin temel amacı, manuel olarak yapılan beton çatlak tespit işlemlerinin otomatikleştirilmesi ile zaman ve emek tasarrufu sağlamak, hata payını azaltmak ve sonuçları daha tutarlı hale getirmektir. Bu sayede, beton yüzeylerin daha hızlı ve etkili bir şekilde değerlendirilmesi sağlanabilir. Ayrıca, beton yapılarda erken çatlak tespiti yaparak, hasarların daha küçük boyutlarda kalmasını sağlayarak onarım maliyetlerinin azaltılmasına da yardımcı olunabilir.
<h2>Veri Seti</h2>
Veriler çeşitli ODTÜ Kampüs Binalarından toplanmıştır. Veri seti, görüntü sınıflandırması için negatif ve pozitif crack görüntüleri olarak ikiye ayrılmıştır. Her sınıf, RGB kanallı 227 x 227 piksel ile toplam 40000 resim olmak üzere 20000 resme sahiptir

![00001](https://github.com/Emircan-Bagdu52/yapayzekaproje/assets/95845060/45f3c744-085f-46fc-a12b-118581802abb)
![00002](https://github.com/Emircan-Bagdu52/yapayzekaproje/assets/95845060/ae5d5fa3-2e4e-4667-ae11-9e1892f0b5c0)<br>
Pozitif &nbsp;&nbsp;&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; Negatif
<h2>Veri Ön İşleme</h2>
Projemizin ilk aşamasında modele girdik olarak vermeden ön işleme adımları uygulayacağız bu adımlar:
<ol> 
    <li>Gri Kanala Çevirme,</li> 
    <li>Filtreleme,</li> 
    <li>Thresoldh</li>
    <li>Motfolojik İşlemler</li>
</ol>
olmak üzere adımdan oluşacaktır. 

Görüntü veri ön işlemede ilk olarak resimleri gri  kanala çeviririz bunun nedeni resimler rgb renk kanalları üzerinde işlenir 3 kanal daha fazla işlem yükü getirir gray kanala çevirerek bize resimleri işleme kolaylığı sağlar. Filtreleme adımı uygulayarak görüntüdeki gürültüleri azaltmak, kenarları vurgulamak veya belirli özellikleri çıkarmak için kullanılır. Threshold(eşikleme) adımıyla görüntü üzerindeki bölgeleri ayırmak için eşikleme değeri belirlenir ve bu değer üzerinden resimler siyah veya beyaz piksel olarak belirlenir son olarak morfolojik işlem, aşındırma ve genişleme. Aşındırma işlemi, nesneleri küçültür ve gürültüyü azaltırken, genişleme işlemi nesneleri büyütür ve boşlukları doldurur. Bu işlemler, görüntüdeki gürültüyü azaltmak ve nesneler arasındaki boşlukları kapatmak için kullandık.
