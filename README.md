# 📑 **Northwind Veri Seti - SQL Senaryoları ve Python Görselleştirmeleri**

![img](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/Northwind%20Data.png)

* **Bitirme Çalışmasının diğer bir ayağı olan SQL ile belirli başlı e-ticaret senaryoları oluşturulmuştur. Bu senaryolara göre bize dört adet Task verilmiş olup bunlarla alakalı sorgular ve görselleştirmeler istenmiştir ancak bu görselleştirmeler python da istenmektedir.**
* **Bu çalışmada MS Access için hayali bir şekilde oluşturulan Northwind Veri seti kullanılmaktadır.**
* **Veri Seti :** [Northwind Veri Seti](https://github.com/pthom/northwind_psql/blob/master/northwind.sql)
* **Çalışmanın Notebook Dosyası :** [Bitirme Projesi Jupyter Notebook](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/Capstone%20Project%20SQL%20Vis..ipynb)

## 📌Veri Seti Tablo İlişkileri ve PostgreSQL ERD :

![img](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/Tablo%20%C4%B0li%C5%9Fkileri.png)
![img](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/ERD.png)
## 📌İstenen Senaryolar : 
🚀**CASE 1 - Tedarikçi Analizi :**

* Satın Alma ekibi, tedarik edilen ürünlerle ilgili ayrıntılı bilgilere ulaşmak ve gerekli aksiyonları almak istiyor. Bu analizde, tedarikçilerin listesi, tedarikçilerin bulunduğu şehirler, her bir tedarikçinin ne kadar benzersiz ürün temin ettiği ve bu ürünlerin hangi kategorilere ait olduğunu görmek istiyorlar. Ayrıca, tedarikçiler bazında ürün sayısı ve toplam ürün tedarik sayısına göre yüzdelik dilimlere ayrılan bilgilere de ihtiyaçları var.

🚀**CASE 2 - Bölge Analizi :**

* Pazarlama ekibi bölgeler baz alınarak sipariş miktarları ve ortalama indirim dahil geliri hesaplamak istemektedirler. Bölgeleri, toplam sipariş sayısı ve indirim dahil ortalama tutarları görmek istiyorlar.

🚀**CASE 3 - Ürün Stok Analizi :**

* Ürün ekibi, envanter analizi yapmak ve ürün bazında ihtiyaçları belirlemek istiyor. Bu kapsamda siparişlerde tekrar edilen ürünleri, yeterli stoku olan ürünleri, satışı devam eden ve sona eren ürünlerin adetlerini görmek istiyorlar. Ayrıca en çok tekrar sipariş edilen ve en fazla stoku bulunan ilk 5 ürünün listesini de talep ediyorlar.

🚀**CASE 4 - Taşıma Şirketi Performans Analizi :**

* Şirket çalıştığı kargo firmalarının ne kadar teslimat yaptığını, ortalama teslimat sürelerini ve müşteri için istenilen ortalama teslimat sürelerini istemektedir. Ek olarak ortalama kargo maliyetleri de istenmektedir.
