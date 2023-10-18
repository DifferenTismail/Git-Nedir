
<div align="center">
  <h1> Git Nedir</h1>
  <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/ismail-baran-karasu-a98916227/">
  <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
  </a>
  <a class="header-badge" target="_blank" href="https://twitter.com/ismaiBaranK">
  <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/ismailBaranK?style=social">
  </a>

<sub>Yazar:
<a href="https://www.linkedin.com/in/ismail-baran-karasu-a98916227/" target="_blank">İsmail Baran KARASU</a><br>
<small> Ekim, 2023</small>
</sub>

</div>
Git, yazılım geliştirme süreçlerinde kullanılan, hız odaklı, dağıtık çalışan bir sürüm kontrol ve kaynak kod yönetim sistemidir. İlk sürümü Linux çekirdeği'nin geliştirilmesinde kullanılmak üzere 2005 yılında bizzat Linus Torvalds tarafından tasarlanıp geliştirilmişdir.

Git sürüm kontrol sistemini kullanan her bir çalışma dizini (proje), internet erişimi ya da merkezi bir depo olmaksızın tüm tarihçeyi tutan ve sürüm kontrol sisteminin tamamını içinde barındıran tam yetkili birer depodur. Aynı çalışma dizininin birçok depodan birindeki kopyasında yapılan değişiklikler diğerlerine güven temelli bir değerlendirmeyle kabul edilir; Güvenilmeyenden değişiklik alınmaz, o kendi ayrı sürümünü geliştirmeye devam eder.

Git'in şu anki yazılım bakıcılığını Junio Hamano üstlenmiş durumda. Git, GNU Genel Kamu Lisansı'nın 2. sürümüyle lisanslanmış bir özgür yazılımdır. 2.26.0 sürümünden itibaren Türkçe dil desteği sunmaktadır.



# Git İle İlgili Temel Kavramlar 
1. Depo (Repository): Git projelerinin temelini oluşturan depo, proje dosyalarının ve sürüm geçmişinin saklandığı yerdir. Bu depo, yerel bir bilgisayar üzerinde veya uzak bir sunucuda bulunabilir.
2. Taahhüt (Commit): Bir taahhüt, projenin belirli bir anında yapılan değişikliklerin bir görüntüsünü temsil eder. Taahhütler, projenin sürüm geçmişini oluşturan temel yapı taşlarıdır.
3. Dal (Branch): Git projeleri genellikle farklı özellikler veya geliştirmeler üzerinde çalışırken farklı dallara ayrılır. Ana dal (genellikle "master" veya "main" olarak adlandırılır), projenin ana sürümünü temsil eder.
4. Birleştirme (Merge): Farklı dallardaki değişiklikleri birleştirme işlemidir. Bu, farklı geliştiricilerin çalışmalarını bir araya getirme veya yeni bir özellik eklerken ana dala dahil etme sürecini içerir.
5. İstemci ve Sunucu (Client and Server): Git, hem yerel bilgisayarlarda çalışabilen bir istemci olarak hem de uzak depolara erişim sağlayabilen bir sunucu olarak kullanılabilir. GitHub ve GitLab gibi hizmetler, uzak sunucular sağlar ve işbirliği yapmayı kolaylaştırır.

# Git Nasıl Kullanılır
## Projeniz için yerel Git deposu (repository) oluşturma
Projeniz yeni olsun veya olmasın tek satır komutla projeniz için Git deposu oluşturabilirsiniz.
Komut ekranını açın ve komut ekranından proje klasörünüze ilerleyin. Projenizin ana klasöründe olduğunuzdan emin olduktan sonra ‘git init’ komutunu girin.

![Project 1](gitinit.PNG)

Projemizde .git adında gizli bir klasör oluşması gerekiyor. Şimdi de ‘git status’ komutunu girelim. Bu komut projemizde en son yapılan kayıttan (commit) sonra yapılan değişiklikleri gösteyor. Biz daha önce herhangi bir kayıt yapmadığımız için de şu an bütün dosyalar yeni birer değişiklik olarak görünmekte.

![Project 2](gitstatus.PNG)

Şimdi de bütün dosyalarımızı kayıt listesine ekleyip ardından da kayıt yapacağız. Bunun için ‘git add .’ komutunu girin. Normalde ‘git add’ komutunun en sonuna eklemek istediğiniz dosyayı belirtirsiniz. Bizim komut sonunda kullandığımız nokta ise bütün dosyaları ekle anlamına gelmekte.

Kayıt işlemi için de ‘git commit -m “ilk kayit” ’ komutunu girin. Bu komutu girdiğiniz anda ekrana projenizdeki bütün dosyaların tek tek eklendiğini belirten satırlar görürsünüz.
