# Araştırma Soruları

Artık yeni iş yerindeki ilk görevini gerçekleştirmek için hazırsın! Kullandığımız araçları biraz daha iyi anlama zamanı. Yapman istenilen şey, bu dokümanı güncelleyerek, aşağıdaki soruları soruları cevaplaman. Böylece Git yapısına biraz daha aşina olmaya başlayacaksın.

Soruları cevaplarken takıldığın yerlerde [GitHub docs](https://docs.github.com/en)'u kullanabilirsin. Docs, (ingilizce documentation'ın kısaltılmış halidir) bir programı veya dilin nasıl kullanılacağını anlatan dokümandır. Yazılım dünyasında sıkça kullanılır. Bir yazılımcı olarak _zamanınızın büyük çoğunluğu da bu tarz dokümanları okumakla ve üzerinde çalışmakla geçecek_.

![READ THE DOCS](https://github.com/Workintech/FSWeb-S1G1-Projesi-Web-Development-Projesi-icin-Git/blob/main/read-the-docs-wit.gif?raw=true)

Eğer aradığın soruların cevapları GitHub docs'ta yoksa, Google'lama becerileriniz size yardımcı olacak. Google'ı iyi kullanabilmek de aslında büyük bir dikkat ve çalışma gerektiriyor. Zamanla bu konuda da daha iyileştiğini göreceksin :)

## Sorular

1. Git nedir?
Git, Açık Kaynak Dağıtılmış Sürüm Kontrol Sistemi(Open Source Distributed Version Control System)'dir.

2. Git ile GitHub arasında ne fark var?
GitHub, bulut tabanlı bir git barındırma hizmeti sunan kâr amaçlı bir şirkettir.versiyon kontrolü ve işbirliği için git kullanımını bireyler ve ekipler için GUI ile kolaylaştırmaktadır.

3. Neden bir branch oluşturuyoruz?
Yazılım yaparken orjinal kaynak kodumuzu korumak amacıyla branch oluşturuyoruz.

4. Pull Request'in amacı nedir?
Diğer geliştiricilere doküman üzerinde değişiklik yapıldığını ve remote repo da bulunan branch e yüklendiğini ifade etmek.

5. Bir Branchten diğerine geçmek için kullandığın KOMUT nedir? Mesela `isim-soyisim` branch'inde çalıştığını hayal et ve main branch'ine geçmek istiyorsun, ne yaparsın?
$ git checkout main

6. `git fetch`, `git merge` ve `git pull` arasındaki farklıarı açıklayınız. Bu konutlar ne yapar açıklayınız.
git fetch : remote repo dan içerik indirmek için kullanılır.Ancak yerel reponun çalışma durumunu güncellemez, mevcut çalışmayı olduğu gibi bırakır.
git pull : Bu komutta remote repo dan içerik indirmek için kullanılır.Ancak daha agresif bir alternatiftir.Çünkü remote repo dan indirilen doküman ile yerel de çalışılan dokümanı birleştirerek günceller.Yani fetch+merge komutlarının birlikte çalışmasıdır.
git merge: iki branch i birleştirir. 

7. Merge conflict nedir?
Bazen birden fazla geliştirici aynı içeriği değiştirmeye çalıştığında (bir dokümanda ki aynı satırı değiştirmeye çalışmak veya bir geliştiricinin üzerinde çalıştığı dokümanın başka bir geliştirici tarafından silinmesi gibi) Git hangisinin doğru olduğuna karar veremez.Buna birleştirme çakışması denir.

8. Merge conflict'i nasıl çözeriz?
git status komutu ile hangi dosya da sorun olduğuna bakarız.
Ardından $ cat 'dosya ismi' komutunu yazarak dosyada ne gibi birleşime engel olan elemanlar var onu tespit ederiz. Ardından da dosyayı bir editor de açarak problemli kısımları kaldırırız. Tekrar merge komutunu çalıştırdığımızda sorun çözülecektir.