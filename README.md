# Joint_Assigments_2

<h1>Öğrenci Notları Tahmini</h1>

<p>Bu repo, çeşitli faktörler kullanarak öğrenci final notlarını tahmin etmek için yapılan analizleri ve kodları içerir. Proje, veri yükleme, ön işleme, keşifsel veri analizi (EDA), model eğitimi ve model değerlendirmesini kapsamaktadır.</p>

<h2>İçindekiler</h2>
<ul>
  <li><a href="#giriş">Giriş</a></li>
  <li><a href="#veri-yükleme-ve-ön-işleme">Veri Yükleme ve Ön İşleme</a></li>
  <li><a href="#keşifsel-veri-analizi-eda">Keşifsel Veri Analizi (EDA)</a></li>
  <li><a href="#model-eğitimi">Model Eğitimi</a></li>
  <li><a href="#model-değerlendirmesi">Model Değerlendirmesi</a></li>
  <li><a href="#sonuç">Sonuç</a></li>
</ul>

<h2 id="giriş">Giriş</h2>
<p>Bu projenin amacı, doğrusal regresyon modeli kullanarak öğrenci final notlarını tahmin etmektir. Veri seti, akademik performansı etkileyebilecek çeşitli demografik ve davranışsal özellikler içermektedir.</p>

<h2 id="veri-yükleme-ve-ön-işleme">Veri Yükleme ve Ön İşleme</h2>
<p>Projeye, iki veri setini (matematik ve Portekizce dersleri için) yükleyerek başlanır. Bu veri setleri ortak özellikler kullanılarak birleştirilir. Veri seti, gereksiz sütunların çıkarılması ve eksik değerlerin işlenmesiyle temizlenir.</p>

<h2 id="keşifsel-veri-analizi-eda">Keşifsel Veri Analizi (EDA)</h2>
<p>EDA aşamasında, farklı değişkenler ve final notları arasındaki ilişkileri anlamak için veri analiz edilir. Bazı önemli analizler şunlardır:</p>
<ul>
  <li><strong>Cinsiyet Karşılaştırması:</strong> Erkek ve kadın öğrencilerin final notlarının karşılaştırılması.</li>
  <li><strong>Çalışma Süresi vs Final Notları:</strong> Çalışma süresinin final notlarına etkisinin analizi.</li>
  <li><strong>Başarısızlıklar vs Final Notları:</strong> Başarısızlık sayısının öğrencilerin final notlarına etkisinin incelenmesi.</li>
  <li><strong>Alkol Tüketimi vs Final Notları:</strong> Alkol tüketiminin akademik performansa etkisinin analizi.</li>
  <li><strong>Devamsızlıklar vs Final Notları:</strong> Öğrenci devamsızlıklarının final notlarına etkisinin gözlemlenmesi.</li>
</ul>

<h2 id="model-eğitimi">Model Eğitimi</h2>
<p>Doğrusal regresyon modeli, ön işlenmiş veriler kullanılarak eğitilmiştir. Veri seti, eğitim ve test setlerine ayrılmış ve model eğitim seti üzerinde eğitilmiştir.</p>

<h2 id="model-değerlendirmesi">Model Değerlendirmesi</h2>
<p>Modelin performansı çeşitli metrikler kullanılarak değerlendirilmiştir:</p>
<ul>
  <li><strong>Ortalama Mutlak Hata (MAE):</strong> Hataların ortalama büyüklüğünü ölçer.</li>
  <li><strong>Ortalama Kare Hata (MSE):</strong> Hataların karelerinin ortalamasını ölçer.</li>
  <li><strong>Kök Ortalama Kare Hata (RMSE):</strong> Hataların karelerinin ortalamasının kareköküdür.</li>
  <li><strong>R<sup>2</sup> Skoru:</strong> Bağımlı değişkenin varyansının bağımsız değişkenler tarafından ne kadarının açıklandığını gösterir.</li>
</ul>

<h3>Performans Metrikleri</h3>
<ul>
  <li><strong>Ortalama Mutlak Hata (MAE):</strong> 3.5465264826446563</li>
  <li><strong>Ortalama Kare Hata (MSE):</strong> 21.428702413016374</li>
  <li><strong>Kök Ortalama Kare Hata (RMSE):</strong> 4.629114467781905</li>
  <li><strong>R<sup>2</sup> Skoru:</strong> 0.006027261013986318</li>
</ul>

<h3>Değerlendirme ve Yorum</h3>
<p>Model, R<sup>2</sup> skoru 0.006 ve hata metrikleri (MAE, MSE, RMSE) ile zayıf bir performans göstermektedir. Bu, modelin tahminlerinin gerçek değerlere iyi uymadığını göstermektedir. Bu sonuçlar genellikle aşağıdaki nedenlerden dolayı ortaya çıkabilir:</p>
<ol>
    <li><strong>Model Yetersizliği:</strong> Model, eğitim verilerini iyi öğrenememiş ve test verileri üzerinde zayıf tahminler yapmaktadır. Bu durumda, model verideki temel kalıpları yakalayamamış olabilir.</li>
    <li><strong>Veri Karmaşıklığı:</strong> Bağımsız ve bağımlı değişkenler arasında lineer olmayan veya karmaşık bir ilişki olabilir ve lineer model bunu yakalayamamış olabilir.</li>
    <li><strong>Yetersiz Özellikler:</strong> Modelde kullanılan özellikler, bağımlı değişkeni doğru bir şekilde tahmin etmek için yeterli olmayabilir.</li>
</ol>

<h4>R<sup>2</sup> Skoru ve Hata Metrikleri</h4>
<ul>
    <li><strong>Ortalama Mutlak Hata (MAE):</strong> Bir tahmin kümesindeki hataların ortalama büyüklüğünü yönlerini dikkate almadan ölçer. Daha yüksek bir değer, tahminlerin daha az doğru olduğunu gösterir.</li>
    <li><strong>Ortalama Kare Hata (MSE):</strong> Hataların karelerinin ortalamasını ölçer, yani tahmin edilen değerler ile gerçek değerler arasındaki kare farklarının ortalamasıdır. Daha yüksek bir değer, modelin daha büyük hatalar yaptığını gösterir.</li>
    <li><strong>Kök Ortalama Kare Hata (RMSE):</strong> Tahmin ve gerçek gözlem arasındaki kare farklarının ortalamasının kareköküdür. Daha yüksek bir değer, hataların daha büyük olduğunu ve modelin performansının kötü olduğunu gösterir.</li>
    <li><strong>R<sup>2</sup> Skoru:</strong> Bir regresyon modelinde bağımsız değişken(ler) tarafından açıklanan bağımlı değişken varyansının oranını temsil eden istatistiksel bir ölçüdür. R<sup>2</sup> skorunun 1.0'a yakın olması, modelin tüm varyansı açıkladığını ve mükemmel bir uyum sağladığını gösterir.</li>
</ul>

<h2 id="sonuç">Sonuç</h2>
<p>Bu proje, öğrenci final notlarını tahmin etmek için doğrusal regresyon modelinin uygulanmasını kapsamaktadır. Model, mevcut verilerle düşük performans göstermiştir, bu da daha fazla özellik mühendisliği ve model iyileştirme gerektirebileceğini göstermektedir.</p>
