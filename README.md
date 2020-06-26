# III-hafta-odevi


1.Task vs process- task vs Thread vs .. ve c# task vs thread vs .. kıyaslamalarını ve task haricinde diğer yöntemler nelerdir araştırınız.
2.Extension Nedir? --> Extra paket ekleme. <br/>
3.SQLite, bunu doğru şekilde (en güncel yol ile) nasıl kullanmalıyız? (Aktif halde kullanıp uygulama)

**Task Nedir?**

**Task**  örneklerinin çalıştırdıkları iş parçalarının belirli süreler boyunca veya süre bağımsız olarak bekletilmeleri istenebilir. Burada zaman bağımlı ya da koşul bağımlı ** ** olarak bekletmelerin / duraksatmaların yapılabilmesi söz konusudur. Amaç işlemleri art arda yapmaktansa birbirinden bağımsız task yaratıp birbirine paralel işlem yaratmak. Bu da bize zamandan tasarruf sağlayacaktır.

**Thread Nedir?**

Thread ler sayesinde birçok işi aynı anda eş zamanlı olarak yapmak mümkündür. Yürütülen iş parçacıklarını bir süre bekletmek  veya istenen anda sonlandırmakta mümkündür.Threading işlemlerini yöneten tipler, .Net Framework tarafında System.Threading alanında barınmaktadır.Threading konusuna başlamadan önce Thread sınıfını tanımak gerekmektedir. Bu sınıf tek bir iş parçacığı nesnesidir. Yani bir iş parçacığını başlatmayı ve süreci yönetmeyi sağlar.

**TASK vs Thread**

Async programlama ile daha sıklıkla kullanılan Task yapısı thread yapısına göre üst seviyededir.Task yapısını kullanarak daha gelişmiş işlemler yapabiliriz. Thread pooling yapısını otomatik olarak kullanıp birbiri ardına eklenebilecek olan işlemleri daha iyi organize etmektedir.

**Thread vs Process**

Threading, aynı ortamda aynı anda birden fazla işi yapmaya denir. Threadler ise bu işlerin her biridir. Threadler aynı anda çalıştığında işlemciye processler olarak gider ve sıraya alınır. Tek çekirdekli işlemcilerde birden fazla thread çalıştığı zaman sırayla threadlerin processlerini işleme alır ve bir thread diğer threadin bitişini beklemeden processleri işlemcide işleme girer. Çok çekirdekli işlemcilerde ise farklı threadler farklı çekirdeklerde aynı anda çalışabilme durumuna sahiptir.

**Extensions**

Extensionlar, yeni özellikler ekleyerek veya mevcut araçları tümleştirerek Visual Studio deneyiminizi özelleştirmenize ve geliştirmenize imkan tanıyan eklentilerdir. Bir uzantının karmaşıklık düzeyi değişebilir ancak temel amacı üretkenliğinizi artırmak ve iş akışı gereksinimlerinizi karşılamaktır.

Uzantıları yüklemek için arama penceresinden arama yaparak yüklemek istediğiniz uzantıyı bularak indir seçilerek işlem yapılır. Bağımlılıkları olan bir uzantıyı yüklemeye çalışırsanız, yükleyici bunların yüklenmiş olup olmadığını denetler. Bunlar yüklenmezse, Uzantıları Yönet iletişim kutusu, uzantıyı yükleyemeden önce yüklenmesi gereken bağımlılıkları listeler.

