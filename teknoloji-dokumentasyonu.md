# Teknoloji dökümentasyonu

---

# Front-end

## Angular
 
 - Google tarafından ortaya çıkarılan ve günümüzde hala gelişmekte olan Angular’ın kullanılmasının en büyük nedenlerinden biri diğer frameworklerden daha esnek kullanışa sahip olması ve modüler kullanım tekniğidir. Bunların yanında içinde bulunan paketlerin hazır olarak gelmesi ve hemen kullanılabilir olması en büyük avantajlarındandır. Performans ve hız bakımından oldukça tatmin edicidir. Bir uygulamanın aynı anda çapraz platformlara hızlıca çıkması isteniyorsa angular bu konuda en büyük yardımcıdır.

 - Angular, React ve diğer modern çerçeveler gibi, HTML'i sunucuda veya hatta bir web çalışanında işleyerek performans kazanımlarından yararlanabilir. Uygulama/site tasarımına bağlı olarak bu eş biçimli işleme, kullanıcının deneyimini daha da anlık hissettirebilir.
Angular için koyabilirsiniz daha yazmadıysanız
 
 
## Angular Material



## CSS/SCSS  

# Back-end

## Quarkus

 - Quarkus OpenJDK ve GraalVM için sektördeki önemli library’leri içinde barındırarak hazırlanmış bir Kubernetes Java Stack. Fakat bunu sadece Kubernetes olarak düşünmeyin bu stack’i herhangi bir platform üzerinde de kullanabilirsiniz.Okuduğum kaynaklarda sürekli olarak Kubernetes Native Java framework olarak vurgulanıyor. Sanırım bu konuda Kubernetes için de-facto olmasını istedikleri için bu şekilde dile getiriliyor.

 - ### Neden Quarkus Kullanmalı?

 - 1. Memory consumption değerleri daha az, düşünün ki daha az memory ile aynı işi yapmak, çok iyi bir tercih sebebi olabilir. İnsanlar Cloud Provider nimetlerinden faydalanırken zaman için şunu fark ettiler, Cost reduction yapmalıyız bu su yakmıyor. <br/>  <br/>
 - 2. Cloud tarafında Serverless Mimarisinin ortaya çıkmasının en önemli nedenlerinden biri Cost Reduction yapmaktı. Gerektiğinde kaynaklar ayakta olmalı, kapalı olduğunda ise; ihtiyaç duyulduğunda çok hızlı bir şekilde cevap vermesiydi. Java tarafında kalmak isteyen organizasyonlar için boot time ne kadar değerli olduğunu tahmin edebiliyorsunuzdur işte bu yüzden Quarkus biçilmiş kaftan olabilir. <br/> <br/>

## Maven

 - Maven genellikle Java platformunda yer alan komutların derlenmesi sırasında kullanılan otomasyon ve inşa aracıdır.

 - Java programlama dili ile uygulama geliştirirken çeşitli kütüphaneler kullanamak isteyebiliriz.

 - Maven proje dosyasına eklenen bağımlılıklar/kütüphaneler ile kolay bir şekilde indirmeyi ve proje yerleştirmeyi sağlar.

 - Kullanılan kütüphaneler proje dosyasında yer aldığından taşınabilirlik sağlanmış olur.

 - Sunmuş olduğu dizin yapısı sayesinde diğer geliştiricilerin projeyi takibini kolaylaşır. 


## GraalVM

 - GraalVM Oracle tarafından geliştirilen bir sanal makine. Java, JVM tabanlı diğer diller, Javascript, Ruby, Python, R, C/C++ ve diğer Low Level Virtual Machine(LLVM) desteği sağlayan dilleri farklı deployment senaryolarında çalıştırabiliyor. LLVM sayesinde adaptörünü yazdığını herhangi bir dili de GraalVM’de çalıştırmak mümkün. Bu yapısıyla polygot mimariler’e tam uyum sağlamaktadır. Ayrıca bellek ve GC optimizasyonları noktasında daha verimli çalıştıklarını iddia ediyorlar, Twitter’ı GraalVM üzerinde çalıştırıyorlarmış.
 
 - GraalVM kullandığı JIT derleyicisinin daha performanslı olduğu iddiasına sahip. Ancak bu yazıda odaklandığımız yeteneği daha çok native image yaratabiliyor olması. Native image, özetle Java tabanlı dillerle AOT kullanabilmek anlamına geliyor. Yani JIT derleyici kullanmadan tamamen optimize bir native base image’a özel kodumuzun derlenmesi ve bu imaj üzerinde çalışması mümkün oluyor.
 
 - Sırtımızdaki yükten nasıl kurtulacağız dediğimiz sorumuzu hatırlarsınız. İşte GraalVM bizim için bu noktada kurtarıcı olarak ortaya çıkıyor. Doğrudan makine koduna derlenmiş kodlar sayesinde uygulamanın açılışı hızlı gerçekleşecek. Ve çalışması esnasında yapılan istatistik toplama, optimizasyon için runtimeda yapılan HotSpot derlemeler vb tüm süreçlerden bizi kurtaracak. Bunların yanında kodun tam performans çalışabilmesi için gereken JVM’in ısınma süresi(istatistik toplama vs hotspot derlemelerin aldığı zaman) tarih oluyor, kod çok hızlı bir şekilde ayağa kalkarken yüksek performansla doğrudan çalışmaya başlıyor.

## Kubernetes

 - Kubernetes Google tarafından GO dilinde geliştirilmiş Cloud Native Computing Foundation tarafından desteklenen mevcut konteyner haline getirilmiş uygulamalarınızı otomatik deploy etmek, sayılarını arttırıp azaltmak gibi işlemler ile birlikte yönetmenizi sağlayan bir Konteyner kümeleme (container cluster) aracıdır.

 - Bulut teknolojilerinin kullanımının yaygınlaşması ile birlikte konteyner kavramı hayatımıza girdi ve önemli hale gelmeye başladı

 - Bu teknolojiyi kullanarak uygulamalarımızı mikroservis mimarisi aracılığıyla daha kolay yönetebilir , daha kolay sorunlarımıza çözüm bulabilir ve daha da önemlisi taşınabilir bir ortam sağladığı için uygulamalarımızı çok kolay bir şekilde taşıyabiliriz.Sürüm geçişlerini de bu sayede kolay bir şekilde yapabiliriz.

## Cassandra DB

 - Cassandra, Java ile geliştirilmiş, açık kaynak(open source), nosql veritabanı tipidir. Okulda öğrendiğimiz Mysql bir ilişkisel veri tabanı mesela. İlişkisel veritabanı alışılagelmiş adıyla RDBMS (Relational Database Managament Systems)’de sorgulama için SQL dili kullanılırken, Nosql’de sorgular yer almıyor. Verilerimiz RDBMS’deki gibi tablolarda tutulmuyor, onun yerine JSON ya da XML formatında column base yapısını kullanarak kaydediliyor. 
 
 - Column base derken Cassandra bir kaç farklı sunucuda üzerinde dağıtık şekilde çalışabildiği için verileri yatay olarak ölçekleyebiliyoruz. Ana makineye bağlı sunucular üzerine kurulu değil bu yapı, sunucu istemci mantığıyla değil de peer to peer mantığıyla çalışıyor. Bütün makineler eşit makinelerden biri çöktüğünde sistem durup diğer makinelerin çalışmasını etkilemiyor.. Bu da kullanımımızı kolaylaştırıyor.

## Hexagonal Architecture

 - Hexagonal Mimari, ortak katmanlı mimari tasarımlarında gördüğümüz bir sistemin çekirdeğini oluşturan temel iş mantıklarının bulunduğu modüler parçaların diğer katmanlarla iç içe olacak şekilde tasarlandığı bu yüzden sisteminizi dışarıya açan katmanların ve temel iş mantıklarını yöneten servis katmanlarının birbirine bağımlı şekilde davranmasına yol açan mimarilerin aksine, katmanlar arasındaki bağımlılığı “domain” dediğimiz tamamen iş mantıklarının olduğu en içte bulunan katmana doğru bağımlı olacak şekilde tasarladığımız Domain-Driver Design mimarisinin özelleşmiş bir versiyonudur

 - Hexagonal Mimaride Kullanılan Temel Prensipler
S.O.L.I.D prensipleri, Robert Cecil Martin(Uncle Bob) tarafından ortaya atılan, geliştirilen yazılımın esnek, yeniden kullanılabilir, sürdürülebilir ve anlaşılır olmasını sağlayan aynı zamanda kod tekrarını önleyen prensipler bütünüdür.
Hexagonal mimaride SOLİD prensiplerden olan “Dependency Inversion Principle” ve “Single Responsibility Principle” esas alınarak tasarım yapılır.<br /><br />
Bu iki prensibi Hexagonal mimaride incelemeye çalışalım.<br /><br />
 - 1. Dependency Inversion Prensibi
Bu prensipte ki temel amacı ortak katmanlı mimari üzerinden kısaca özetleyecek olursak bir kod bloğunun, sınıfının, metodunun ya da özelliğin onu kullanan diğer alt kod bloklarına karşı bağımlılığını minimize etmektir. Bir başka deyişle sisteminizdeki alt katmanlarınıza olan bağımlılığı azaltıp bağımlılığı üst katmanlara doğru yönlendirmektir.
Peki hexagonal mimaride “Dependency Inversion” prensibini nasıl uygulamaktayız?
Hexagonal mimaride ortak katmanlı mimarinin en üst katmanı olan domain aslında en içerdeki katmandır. Durum böyle olunca sistemin bağımlılıkları dışardan içe doğru olacak şekilde tasarlanır. Aşağıdaki şekil üzerinden bunu açıklamaya çalışalım:


 - - Sol tarafta ortak katmanlı mimari dediğimiz, üst katman olan domainin yani temel iş mantıklarının gerçekleştiği katmanının persistence dediğimiz veritabanı işlemlerinin bulunduğu katmana bağımlı kaldığını görüyoruz.
Sağ taraftaki tasarımda ise ortak katmanlı mimaride iş mantıklarını manipüle eden servis use-case’ lere ayrıştırılmış durumda. İş mantıklarının persistence katmanı ile olan bağımlılığının ortadan kalktığını, bağımlılığın dıştan içe doğru başka bir deyişle domain katmanına doğru uygulandığını ve domain katmanın aslında izole bir şekilde durduğunu görebiliyoruz.<br /><br />
 - 2. Single Responsibility Prensibi
Bu prensipte bir kod bloğunun, sınıfının, metodunun ya da özelliğin değişimi tek bir sebepten dolayı yapılabilir. Bu durumu gene yukarıda Şekil 1' de çizdiğimiz yapı üzerinden açıklamaya çalışalım. Sol taraftaki tasarımda persistence ya da domain katmandaki bir değişiklik beraberinde birden fazla katmanda değişikliğe sebep olurken, sağ taraftaki tasarımda domain ya da persistence katmanındaki değişiklik sadece kendi tarafında değişikliğe sebebiyet vermektedir.<br /><br />

- ### Temel bileşenleri
1. Domain
Domain için sadece iş kurallarından oluşan, bu kuralların entity’ler vasıtasıyla tanımlandığı ve işlendiği, uygulamanın hiçbir katmanı ile bağımlılığı olmayan aslında uygulamanın temel işlevinin ne olduğunu anlamamızı kolaylaştıran saf kod blokları diyebiliriz. ”Single Responsibility” prensibinde yukarıda anlattığımız gibi dış katmanlardaki herhangi bir değişiklik domain’i etkilemez.
Domain veritabanı, web, UI, job vb dış dünyaya açık olan akışlardan izole edilmelidir.<br /><br />
2. Use-Case
İş kurallarını etkileyen, uygulamayı çağıran birincil portların kullandığı senaryoları içeren ve ortak katmanlı mimaride gördüğümüz servis kısmında bulunan senaryoların tek tek ayrıştırılmış hali diyebiliriz.
Hexagonal mimaride bir use-case aşağıdaki 4 temel görevi yerine getirir:
Input adaptörler aracılığıyla dış sistemden veriler alır.
Domainde tanımladığımız iş kurallarının validasyonunu sağlar ve bunu domaindeki entityler ile paylaşır.
Input değerlerine göre domaini manipüle eder.
Domain objesinin durumu güncellendikten sonra çıkış verisini oluşturur.
Bir use-case, domainde olduğu gibi uygulamanın core katmanında bulunur ve dışardaki katmanlarla bağımlılığı bulunmaz.<br /><br />
3. Input & Output Ports
Domain ve use-case ’ler hexagonal mimaride uygulamanın core tarafını oluşturur. Uygulamanın dışarı ile iletişimi input ve output portları üzerinden gerçekleşir.
Bir input port, uygulamadaki use-case tarafından implement edilen basit bir arayüzü ifade eder. Dış katmanda bulunan bir input adaptör tarafından çağrılarak uygulamanın dışarı ile iletişimene olanak sağlar.
Bir output portu, uygulamanın dışarıdan bir şeye ihtiyaç duyması halinde use-case tarafından çağrılabilen basit bir arayüzdür. Örneğin, veritabanı erişimini yapan ve use-case ’in ihtiyacı olan veriyi elde etmemizi sağlayan basit bir arayüzü düşünebiliriz. Output port dış katmanda bulunan bir output adaptör tarafından implement edilir. Böylece use-case ’in dış ortama bağlılığı ortadan kalkmış olur.
Ayrıca input ve output portları sayesinde bir sisteme verinin nerden geldiğini ve sistem tarafından oluşturulan verilerin nasıl dışarıya aktarıldığını rahatlıkla tespit edebiliriz.<br /><br />
4. Input & Output Adapters
Hexagonal mimaride adaptörler en dıştaki katmanları oluşturur. Uygulamanın çekirdeğinin bir parçası değillerdir fakat input ve output portları üzerinden dolaylı olarak uygulama ile iletişime geçerler.
Input adaptörlere bir web arayüzü ya da bir job örnek verilebilir. Bu adaptörler input portlarını çağırarak uygulamanız üzerinde bir istek oluştururlar.
Output adaptörler ise output portlarını implement eder ve bir use-case üzerinden çağrılırlar. Bir veritabanına bağlanıp veriyi kaydetme ya da veriyi okuma işlemi örnek gösterilebilir.
Hexagonal mimari, bir uygulamanın kolay geliştirilebilmesine ve kolay deploy edilebilmesine, bakım maliyeti az olan sistemlerin tasarlanmasına, eğer ekip olarak bir ürün üzerinde çalışıyorsanız aynı perspektif ile ürüne yaklaşmanıza olanak sağlayan bir mimari modeldir.