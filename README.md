# ProgrammingWithCsharp
C# çalıştığım alan.

## Gün 1

Bugünkü komutlar:

#Github reposundan proje klonlamak için --> git clone https://github.com/kaannerenn/ProgrammingWithC-.git

#Yeni bir solution açmak için --> dotnet new sln

#Git reposuna kodları göndermek için --> git push

#Git reposundan kodları çekmek için --> git pull

u bölümde dersler sırasında işlenen konuları pekiştirmek amacıyla kullanılabilecek bazı örnek senaryolara yer verilmektedir. Kodlama pratiğinin artırılması için kullanılabilir.

Senaryo Kodları : Y -> Yellow (Yani hafifsiklet kod parçaları), O -> Orange (Orta seviye senaryolar) , R -> Red (Bizi iyice zorlayacak senaryolar)

Kod	Konu	Açıklama	Kurallar
Y00	Nesne Modellemeleri(Class)	Okuduğunuz kitaplar için bir envanter uygulaması geliştirmektesiniz. Bir kitabın nesnel olarak moddellenmesinde kullanılacak tasarıma ihtiyacınız var. Bu anlamda sizden Book isimli bir sınıf tasarlamanız bekleniyor.	int, string, bool, decimal veri türleri mutlaka kullanılmalı. Kod, bir kitabın bilgilerini string türde özetleyen, kitap fiyatına indirim uygulayan en az iki metot içermeli.
Y01	Value Type Tasarlaması(Struct)	Geliştirmekte olduğumuz iki boyutlu oyunda Vektör değerlerini tutmak istiyoruz. Bunun için bir struct tasarlamanız bekleniyor.	Struct 2 boyutlu düzlemde mutlaka x ve y değerlerini taşımalı. double veri türü kullanılmalı. Bir vektörü birim vektöre dönüştüren, vektör bükülüğünü hesap eden en az iki metot yazılmalı
Y02	Terminal ile Çalışmak	Bu çalışmada bir Console uygulaması oluşturup ekrana en sevdiğiniz çizgi roman/kitap karakterinin bilgilerini yazdırmanız bekleniyor.	Karaktere ait tüm bilgiler öncelikle ayrı değişkenlerde toplanmalı. string, double, char, bool, uint veri türleri mutlaka kullanılmalı. Bilgileri ekrana yazdırma operasyonunu bir metot üstlenmeli
Y03	Enum Türü Kullanımı	Bir web uygulamasının backend tarafında kodlama yapıyorsunuz. İş kurallarını işleten bazı fonksiyonlar HTTP durum kodları ile çalışıyor. HTTP durum kodlarının sayısal anlamlarını bir Enum sabiti olarak tanımlamanız bekleniyor.	Enum sabiti HTTP durum kodlarından en az 5ini karşılamalı. Uygulama kodunda Enum değerine göre ekrana bilgilendirme yapmamızı sağlayacak string türden değer döndüren bir metot bulunmalı.
Y04	Metot Kullanımları	Termianale farklı desenelerde çıktılar veren bir metot geliştirmemiz isteniyor. Örneğin "Merhaba Dünya!" için "m_e_r_h_a_b_a d_ü_n_y_a_!" yazması vb	Parametre olarak stili değiştirilecek string değer alan ve geriye string değer döndüren bir metot olması bekleniyor. Metot parametre olarak nasıl bir formatta çıktı hazırlayacağını da argüman olarak alabilir.
Y05	Döngülerin Etkin Kullanımı	Elimizde birden fazla şehir bilgisinin tutulduğu bir sınıf olduğunu düşünelim. Bu şehir bilgileri List türünden bir koleksiyonda tutuluyor olsunlar (Reporter sınıfına benzer) Belli mevsimlere göre sıcaklık ortalamalarının altına veya üstünde kalan şehirlerin listesini döndüren bir metot yazmamız bekleniyor	Reporter sınıfını baz alabiliriz. List koleksiyonlarının arama işlemleri için zengin metotları vardır ancak bunları kullanmayalım. Basit for veya while, do...while gibi döngülerden yararlanalım.
Y06	Interface Kullanımının Temelleri	Masaüstü uygulamalar geliştirmemizi sağlayan bir program üzerinde çalıştığımızı düşünelim (Visual Studio kod editörü gibi) Senaryoda AzonButton, AzonImageButton, AzonRadioButton, AzonGridButton gibi kendi sınıflarımız olsun. Tüm bu sınıflar için ekrana çizdirme (Render) operasyonunu ortak bir davranış olarak tasarlayalım. Draw operasyonu içeren tüm bileşenler için topluca bu işlevi çalıştıracak döngüyü içeren metodu yazmayı deneyin.	Tüm button kontrollerinin Draw operasyonunu kendince işletmesi ve mutlak suretle içermesi gerekmektedir. Button kontrolleri bizim tarafımızdan tasarlanan basit entity sınıfları olarak düşünülebilir. Id, Position, Text gibi özellikleri olabilir kendilerine has metotları da bulunabilir.
Y07	Exception Durumları	Depo envanterinde olan ürünlerin yönetildiği bir uygulama kodu üzerinde çalıştığınızı düşünün. Inventory isimli sınıfızda farklı kategorilerdeki ürünlerin stok bilgileri de tutuluyor. Stok bilgileri için ayrı bir veri yapınız var. Stoktaki ürün sayısının eksi değer girilmesi halinde ortama InvalidProductCountException isimli bir exception nesnesi fırlatmanız bekleniyor.	Stok bilgilerini tutan sınıfta kateogori numarası, ürün numarası ve güncel ürün sayısı bilgilerini tutabilirsiniz. Inventory sınıfı bu stok sınıfına ait nesne örneklerinin koleksiyonunu taşımalıdır. Fırlatılan Exception runtime' da (Console uygulaması olarak tasarlanabilir) yakalanmalıdır.
Y08			
Y09			
Y10			
Y11			
Y12	Test Pratikleri	Test Driven Development pratiklerinin kazanılması için yapılan çeşitli kod kataları vardır. Bunlardan birisi de Fizz Buzz problemidir. 0dan 100e kadar sayan bir metot 3 ve 5 ile bölünebilen sayılara bakar. 3 ile bölünenler için ekrana Fizz, 5 ile bölünenler için Buzz, hem 3 hem de 5 ile bölünenler için FizzBuzz yazar. İstenen şey bu metodu test driven development yaklaşımı ile yazmaktır.	XUnit türünden bir test projesi üzerinde geliştirilmelidir. Proje en az 5 test metodu içermelidir.
O01	Polimorfik Nesnelerin Keşfi	Bu çalışmada bir oyunun anlık halinin kayıt edilmesi üzerine bir süreç söz konusudur. Bir oyunda sahadaki nesneleri yöneten nesnenin kayıt işlemini çalışma zamanından önce belirlenen ortama yazması beklenir. Bazı durumlarda metin tabanlı bir dosyaya bazı hallerde cloud ortamındaki bir servise veya veri tabanına yazdırabilir.	Buradaki tek kural oyun sahasındaki nesneleri tutan container bileşeninin yazma operasyonunu değiştirmek için kodunu değiştirmeden hareket edilmesi gerekliliğidir. Yani kaydetme davranışının değişime kapalı ama genişletilmeye açık bir şekilde tesis edilmesi beklenmektedir. Bu davranış genişletmesi için Interface kullanımı zaruridir
O02	Metinsel Veri Manipülasyonları	Elimizde şöyle bir metinsel içerik olduğunu düşünelim. {html}{body}{head}Product Info{head}{p}Title: {@model.Title}{p}{br}{p}Description : {@model.Description}{br}{p}List Price : {@model.ListPrice}{p}{body}{html} Yazacağımız bir runtime da @model ile başlayan yerleri gerçekten bir Product sınıfının verileri ile değiştirmek istiyoruz. Bunu işleten metotu yazmayı deneyiniz	Ortamda bir Product sınıfı olmalı ve ayrıca belirtilen metinsel ifade bir text dosyadan okunmalı. Metodumuz text tabanlı dosyayı almalı ve burada @model ile başlayan kısımları tespit edip doğru Product nesne özellikleri ile değiştirebilmeli.
O03	Serileştirme İşleri	Video oyunları ile ilgili bir almanac üzerinde çalışıyoruz. Kullanıcıdan gelen bilgileri alan ve bunları toplayan bir container nesnemiz bulunuyor. Bu container nesnenin oyunlara ait veri koleksiyonlarını JSON formatında serileştirip kaydetmesini ve gerektiğinde kaydedilmiş dosyadan ters serileştirme usulüyle okumasını bekliyoruz.	Newtonsoft paketi yerine .Net in built-in JSON serileştirme modülü kullanılmalı. Oyunlarla ilgili title, summary, category, release year, popularity point, in stock, platform gibi bilgiler tutulabilmeli. Girişler terminal ekranından yapılabilmeli ve kullanıcı istediği kadar oyun bilgisi girebilmeli. Oyun girdilerinde veri türü kontrolleri mutlak suretle yapılmalı.
O04	Genişletme Fonksiyonellikleri	Bir nesne topluluğu üzerinde filtreleme, sıralama, veri ayrıştırma gibi bazı işlemleri gerçekleştirmek istiyoruz. Burada istenilen türden bir nesne koleksiyonu tasarlanabilir. Bahsedilen fonksiyonellikler içinse LINQ (Language INtegrated Query) sorguları haricinde kendi tasarladığımız metotlardan faydalanılmalıdır.	LINQ ile gelen hazır fonksiyonlar yerine kendi tasarladığımız metotların kullanılması gerekiyor.
O05	Yeniden Terminale Dönüş	Sarı kategoride yer alan 4 numaralı örnek (Y04) program kodunda bir metnin ekrana farklı stillerde yazdırılması için gerekli işlemleri ele alıyor. Yazı stillerine göre işlemlerin nasıl yapılacağı enum sabiti değerlerine karşılık gelen fonksiyonlarda işlenmekte. Ancak yeni bir yazı stili eklenmek istediğimizde WriteBeauty metodunun kodunu değiştirmemiz gerekmekte. Bu kodu değiştirmeden yeni bir yazı stilini Terminal sınıfına nasıl öğretebiliriz?	Örnek çözümde Dependency Inversion prensibinin mutlak suretle kullanılması gerekiyor. Component ilişkisini kurarken Interface kullanımı da gereksinimlerden birisi.
O06			
O07			
O08			
O09			
O10			
O11			
O12			
R01	Plug-In Tabanlı Geliştirme	Bu senaryoda bir programın kodunun değiştirilmeden genişletilebilmesi ele alınır. Örneğin bir grafik uygulamasının standart kütüphanesinde temel resim fonksiyonlarını sunduğunu düşünelim. Gölgeleme, siyah beyaza çevirme gibi efektleri işeten fonksiyonlar olarak düşünebiliriz. Amacımız yalın bir SDK geliştirmek ve buradan sunacağımız imkanlarla bu SDK'yi kullanan taraflara kendi efektlerini de ekleyebilmelerini sağlamak.	Bu örneklte SDK görevi gören bir Class Library, bunu kullanan hayali bir grafik uygulaması (terminal tabanlı geliştirilebilir) söz konusudur. SDK kullanıcısı kendi efektini runtime'a öğretmek için SDK'yi baz alır. Grafik çizim uygulaması (terminal uygulaması olduğunu bir kez daha hatırlatalım) yeni efektleri, SDK'den geliştirilen yeni Class Library' yi kullanarak ele alabilir. Önemli kural, grafik uygulaması (runtime sahibi) yeni efektleri içeren (ve bunun için SDK kütüphanesini referans eden) kütüphaneyi referans etmeden kullanmalıdır.
R02	Nesne Bağımlılıklarını Gevşetmek	Bir bayi otomasyon sistemindeki faturalama süreçlerinin ele alındığı bir modülde geliştirici olarak çalıştığınızı düşünün. Faturanın kendisini bir model nesnesi olarak tasarladınız ve bir başka bileşeniniz de fatura kesme işini üstleniyor. Bir fatura kesildiğinde müşteriye bildirim gönderilmesi isteniyor ancak bu bildirimin nasıl yapılacağı belli değil. SMS ile olabilir, E-Posta gönderimi olabilir, Whatsapp mesajı olabilir veya push notification tarzı yeni bir hizmet kullanılabilir. Bu işin Fatura kesme işini üstlenen component'ten soyutlanarak dışarı alınması ve gevşek bağlı bir bileşen halinde tasarlanması bekleniyor. Senaryo gereği bu gönderim işlemlerinden birden fazlası aynı anda yapılabilir. Yani hem SMS hem e-posta gönderimleri de söz konusu olabilir. Dolayısıyla bileşen bağımlılığının birden fazla dış enstrümanı kullanacak şekilde tesis edilmesi gerekiyor.	Yeni bir gönderim şeklini sisteme eklerken veya önceden tanımlanmış olanları kullanırken fatura kesme operasyonunu üstlenen bileşen kodunda değişiklik yapmamamlıyız.
R03	Performanslı İçerik Üretmek	Bir projede test verisi üretmemiz isteniyor. Test verileri rastgele metinsel içeriklerden oluşan ancak boyutları 2 ila 5 Mb arasında değişen dosyalar olmalı. Dosya sayısı istenen test kümesi için ayrılan fiziki disk alanına göre belirlenmekte. Örneğin 500 Mb lık bir test içeriği için 100 tane 5 mb'lık dosya üretmek gibi. İstenen şey bu üretim işinin mümkün mertebe en hızlı biçimde yapılması.	Dosya üretme işlerini üstlenen bir runtime geliştirilmeli ve dosyalar sıralı olarak değil eş zamanlı olarak üretilebilmeli ve ayrıca her dosyanın içeriği farklı olmalı. Her dosya PREPARED FOR TEST PURPOSE ifadesi ile başlamalı ve bitmeli.
	
