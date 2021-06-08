# Reinvest Düğmesi

## Reinvest düğmesine basmam gerekiyor mu?

Hayır. Bir başkası ödülü kazanmak için sizin yerinize basacaktır.

## Nasıl Çalışıyor?

Reinvest düğmesi havuzdaki herkes için biriken tüm ödülleri alır ve işlem çiftindeki iki tokena çevirerek poola tekrar yatırır. 

Reinvest butonuna basmak için havuza göre değişen oranda bir teşvik ödülü vardır. Her kim düğmeye ilk basarsa ödülü alır ve herkes için havuza geri yatırır.

## Ne Zaman Basmalıyım?

Reinvest düğmesi opsiyoneldir. Basmak zorunlu değildir. Ancak ödül almak isteniyorsa basılabilir.

Eğer amaç Avaxa karşı net bir kazanç sağlamaksa, ödül tokenı ve Avax fiyatı oranı, havuza reinvest için gereken gas maliyeti ve ödülü satıp Avaxa çevirmek için gereken gas maliyeti hesaba katılmalıdır. 

Reinvest düğmesine basmak ve ödülü almak için havuzda yatırım sahibi olmak gerekmez. Düğmeye basan ve transferi gerçekleştiren herkes ödülü alabilir. Ancak reinvest butonunda rekabet yüksektir ve  biraz hızlı olmak gerekebilir.

## Reinvest Sürecine Bir Örnek

Örnek olarak diyelim ki aşağıdaki havuzdasınız \(Pangolin ETH-AVAX / PEFI\). 

![](../.gitbook/assets/screen-shot-2021-05-14-at-9.06.18-pm.png)

Bu havuza ETH ve AVAX ikilisine Pangolinde likidite  sağlayarak, sonra da havuz tokenlarını Yield Yak'a yatırarak dahil oldunuz. Bu havuz tokenları Yield Yak tarafından Penguin Finance'e yatırılarak karşılığında PEFI ödülleri toplanır. 

Sonra birisi gelerek 100 tane PEFI ödülü biriken bu havuzun reinvest düğmesine basar,

* Reinvest düğmesine basan kişi 3 PEFI alır \(ödül %3 olursa\)
* Yak hazinesi 5 PEFI alır\(hazine hakkı %5'se\)
* Kalan 92 PEFI geri havuza yatırılır.

Kalan 92 PEFI, ETH ve AVAX'a karşı satılıp tekrar Pangolin'de likiditeye eklenir ve YAK havuzuna tekrardan yatırılır.

## Daha fazla bilgi

### Koruma Mekanizması

Reinvest fonksiyonu, iki reinvest işleminin arasındaki süreyi kısıtlamak için bir koruma mekanizması barındırır. İkinci reinvest eylemi\(neredeyse hiç ödül alamayacak olan\) tam komisyon ücreti harcamaktansa çok daha düşük bir komisyon ücretiyle\(0.03 AVAX\) başarısız olur. 

Eğer bir başkası sizden daha hızlı olduğu için hiç ödül alamadıysanız ve reinvest eyleminiz tam komisyonla gerçekleştiyse lütfen ekibe değişiklik önerisinde bulunun.

### Başarısız Transfer

Reinvest butonuna bastıktan sonra transfer hatasıyla karşılaşırsanız bunun temelde iki nedeni olabilir. 

1. Bir şekilde token ödülü min. limitin altındayken transfer yapmayı başarmışsınızdır. Eğer durum buysa gas çok düşük olacaktır\(0.03 AVAX\) 
2. Bir sebepten dolayı Reinvest için kullanılan standart gas limiti transferi gerçekleştirmek için yeterli olmayabilir. Bu durumda gas limitini manuel olarak arttırmanız gerekir. Bundan dolayı oluşacak hata tüm standart gas limitiniz kadar miktarı kaybetmenize sebep olabilir.

### Komisyonlar

Komisyonlar her reinvest tuşuna basıldığında ödül tokenları üzerinden toplanır.

Komisyonlar genelde 5-10% arasındadır. Komisyon oranları ağın durumuna göre ödülü optimize etmek için değişebilir. Komisyonlar 3 parça halindedir.

1. **Reinvest Ödülü** - reinvest tuşuna basan kişiye ödenir
2. **Yönetici komisyonu** - ağa ödenir
3. **Geliştirici komisyonu** - stratejiyi yazan geliştiriciye ödenir

Yield Yak herhangi bir yatırma ve çekme komisyonu talep etmez\(temeldeki havuzların bu yönde talepleri olabilir\)

  

