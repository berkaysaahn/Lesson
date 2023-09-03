### HTML Nedir ?
HTML(Hyper Text Markup Language), bir programlama dili değil işaretleme dilidir. WEB tarayıcısı tarafından çözümlenir, metin ve görselleri istenilen sayfalara yükler. Dilin en son sürümü HTML5'tir. 1993 yılında [[CERN]]'de [[Tim Berners-Lee]] tarafından CERN içerisindeki araştırmacıların dökümanları birbirleri ile paylaşmaları için tasarlanmıştı ama daha sonraları dünya çapında paylaşım gerçekleşmiştir. 

HTML kodlarına etiket adı verilir, açık ve kapalı etiketler bulunur. Açık etikete örnek olarak br etiketi verilebilir bu etiket /br ile kapatılmaz. Kapalı etikette ise etiket <> arasına yazılır ve </> arasına alınarak kapatılır.

### HTML'e Giriş
Dosya oluşturulduktan sonra ilk işlem olarak web tarayıcısı için HTML'in sürümü belirtilir. HTML5 için bu belirtme işlemi "!DOCTYPE html" şeklindedir. 
Bu belirme işleminden sonra "head" etiketi oluşturulur ve bundan sonraki tüm etiketler bu etiketin altında bulunur.
html etiketinden sonra ilk olarak "head" etiketi oluşturulur. head etiketi, bir HTML belgesinin başlık, meta veriler, stil tanımlamaları ve diğer sayfa seviyesi bilgileri içeren bölümünü tanımlayan bir HTML öğesidir. Şimdilik satece title etiketi ile sayfanın başlığını oluşturmamız yeterlidir.
Daha sonrası "body" etiketi oluşturlur. Bu etiket arasında kalanlar sayfanın görsel ve metinsel düzenlemesi ile alakalı etiketlerdir.

#### b, strong, i, u, br, h Etiketleri
Bu etiketlerin tümü "body" etiketinin altında bulunur.
1. <b>b Etiketi:</b> Bu etiket kapatılan bir etikettir ve arasında bulunan metni görsel olarak kalınlaştırır.
2. <b>strong Etiketi:</b> Bu etiket arasına gelen metni vurgulamak için kullanılır. b etiketi ile çok benzerdir.
3. <b>i Etiketi:</b> i etiketi arasına gelen metni italik olarak gösterir.
4. <b>u(underline) Etiketi</b> u etiketi arasına gelen metnin altını çizmeye yarar.
5. <b>br(break) Etiketi:</b> br etiketi bir sonraki satıra geçmeye yarar.
6. <b>h(heading) Etiketi:</b> h etiketi numaralı ve kapanan bir etikettir h1, h2... gibi devam eder, başlık oluşturmak için kullanılır.

#### font Etiketi ve Parametreleri
font etiketi ile metin düzenlemesi yapılır. Parametreleri aşağıda verilmiştir:
1. <b>color Parametresi:</b> color parametresi ile yazımıza renk veririz. RGB kodları kullanılarak özel renkler verilebilir.Başlarına # işareti konulur, ff0000 ile kırmızı 00ff00 ile yeşil 0000ff ile mavi oluşturulur ve bu üç renk karılabilir.
2. <b>size Parametresi:</b> size parametresi ile yazımızın boyutunu ayarlarız.
3. <b>face Parametresi:</b> face parametresi ile yazının şeklini ayarlarız. Örnek olarak Arial verilebilir.
#### img Etiketi ve Parametreleri
img(image) parametresi ile sayfamıza resim ekleyebiliriz. Parametreler aşağıda verilmiştir:
1. <b>src(source) Parametresi:</b> src parametresi kullanılarak yüklenecek resmin dizin yolu belirtilir.
2. <b>width Parametresi:</b> width parametresi ile resmimizin genişliği belirtilir.
3. <b>height Parametresi:</b> height ile yükseklik belirtilir. Eğer width veya height parametrelerinden herhangi biri verilir ve diğeri verilmezse otomatik oluşur.
4. <b>title Parametresi:</b> title parametresi ile resmimizin üzerine gelindiğinde ne yazmasını istiyorsak onu belirtiyoruz.
5. <b>alt(alternative) Parametresi:</b> img etiketi için en değerli parametredir. Alternative anlamına gelir ve resmin alternatif ismini belirtmek için kullanılır. Bu parametre kullanıldığında resmin görüntülenemediği durumlarda resmin yerine gösterilecek olan metni belirtir. alt parametresi arama çubuğuna yazılan kelimenin aramalar ve görsel aramalarda çıkması için web tarayıcısı tarafından kullanılır, bu yüzden değerli bir parametredir.
6. <b>border Parametresi:</b> border parametresi ile resmimize çerçeve veririz ve kalınlık belirtmek için sayısal değerler girilir.

#### Sıralı ve Sırasız Liste Oluşturma
Sıralı liste için ol(ordered llist) etiketi kullanılır, sırasız liste için ul(unordered list) etiketi kullanılır. Her ikisi içinde(ul ve ol) liste elemanları li(list item) etiketi ile verilir. 

> [!Example] Örnek
> -ol type="I" start="3"-
> -li- Beşiktaş -/li-
> -li- Fenerbahçe -/li-
> -li- Galatasaray -/li-
> -/ol-


> [!example] Örnek
> -ul type="disc"-
> -li- Bursaspor -/li-
> -li- Trabzonspor -/li-
> -li- Beşiktaş -/li-
> -/ul-

ol etiketinin type parametresi ile 1(varsayılan), I, a argümanlarını alabilir.
ul etiketinin type parametresi ile disc(varsayılan), circle, square argümanlarını alabilir.

#### a Etiketi ve Parametreleri
a(anchor) etiketi ile link verilerek sayfa içerisinde veya dışarısında farklı bir alana yöneltilir. Parametreleri aşağıdaki gibidir:
1. <b>href(hypertext reference):</b> Hipermetin bağlantısı bu parametre ile tanımlanır. İstenilirse dosya yolu istenilirse URL verilerek yapılabilir. Sayfa içinde tanımlı bir metne gidilmek istenirse de bu parametre kullanılır.
2. <b>target Parametresi:</b> target parametresi ile linkin nerede açılacağı belirlenir: (alt tire)self ile bağlantı mevcut pencerede yüklenir varsayılan değerdir, (alt tire)parent ile bağlantı bağlantıyı içeren çerçevede yüklenir, (alt tire)top ile bağlantı çerçeve dışında kalan heryerde açılır, (alt tire)blank ile bağlantı yeni bir pencerede açılır.

> [!example] Örnek
> -a href="~/Kodlar/html/uygulama1.html" target="_blank"- Uygulama1 -/a-
