# 📑 **Northwind Veri Seti - SQL Senaryoları ve Python Görselleştirmeleri**

![img](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/Northwind%20Data.png)

* **Bitirme Çalışmasının diğer bir ayağı olan SQL ile belirli başlı e-ticaret senaryoları oluşturulmuştur. Bu senaryolara göre bize dört adet Task verilmiş olup bunlarla alakalı sorgular ve görselleştirmeler istenmiştir ancak bu görselleştirmeler python da istenmektedir.**
* **Bu çalışmada MS Access için hayali bir şekilde oluşturulan Northwind Veri seti kullanılmaktadır.**
* **Veri Seti :** [Northwind Veri Seti](https://github.com/pthom/northwind_psql/blob/master/northwind.sql)
* **Veri Setinin içeriğinde müşteriler, tedarikçiler, taşıma şirketleri, ürünler ve bu ürünlerin ait olduğu kategoriler, ürünlerin kargo maliyetleri, fiyatları, satılan adetleri vs. gibi birçok veri bulunmakta ve tamamen gıda ürünlerine ait birbirinden farklı challengelar sunmakta bizlere.**
* **Çalışmanın Notebook Dosyası :** [Bitirme Projesi Jupyter Notebook](https://github.com/hamzaugursumer/CapstoneProjectKodlasam-2/blob/main/Capstone%20Project%20SQL%20Vis..ipynb)

## 📌**Veri Seti İçerisindeki Tablalar ve Sütun Açıklamaları :**

* **Tablo Adı: CATEGORIES**

---------------------------------
| Sütunlar      | Açıklama       |
| ------------- | -------------- |
| CategoryID    | Bu sütun, kategorileri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| CategoryName  | Bu sütun, kategorinin adını içerir. Örneğin, "Beverages", "Dairy Products" gibi kategori adları içerebilir. |
| Description   | Bu sütun, kategorinin açıklamasını içerir. Kategorinin ne tür ürünleri veya hizmetleri kapsadığına dair metin bilgisi sağlar. |
| Picture       | Bu sütun, kategorinin resim veya simgesini içerebilir. Görsel bir temsil sağlar ve genellikle bir bağlantı veya resim verisi içerir. |
---------------------------------

* **Tablo Adı: CUSTOMERS**

| Sütunlar     | Açıklama                                                                                    |
|--------------|---------------------------------------------------------------------------------------------|
| CustomerID   | Bu sütun, müşterileri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| CompanyName  | Bu sütun, müşterinin şirketinin adını içerir. Örneğin, "ABC Ltd.", "XYZ Şirketi" gibi şirket isimleri içerebilir. |
| ContactName  | Bu sütun, müşteri ile iletişim kurulacak kişinin adını içerir. Bu kişi genellikle şirketin temsilcisi olabilir. |
| ContactTitle | Bu sütun, iletişim kişisinin unvanını içerir. Örneğin, "Satış Müdürü", "CEO" gibi unvanlar içerebilir. |
| Address      | Bu sütun, müşterinin adresini içerir. İşyeri veya ev adresi gibi fiziksel konum bilgilerini içerir. |
| City         | Bu sütun, müşterinin bulunduğu şehri içerir. |
| Region       | Bu sütun, müşterinin bulunduğu bölgeyi içerebilir. Örneğin, eyalet veya ilçe bilgisini içerebilir. |
| PostalCode   | Bu sütun, müşterinin posta kodunu içerir. Posta kodu, coğrafi konumu belirlemek için kullanılır. |
| Country      | Bu sütun, müşterinin bulunduğu ülkeyi içerir. |
| Phone        | Bu sütun, müşterinin telefon numarasını içerir. İletişim için kullanılır. |
| Fax          | Bu sütun, müşterinin faks numarasını içerebilir. İhtiyaç halinde iletişim için kullanılır. |
---------------------------------
* **Tablo Adı: EMPLOYEES**

| Sütunlar        | Açıklama                                                                                        |
| --------------- | ----------------------------------------------------------------------------------------------- |
| EmployeeID      | Bu sütun, çalışanları benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| LastName        | Bu sütun, çalışanın soyadını içerir. |
| FirstName       | Bu sütun, çalışanın adını içerir. |
| Title           | Bu sütun, çalışanın unvanını içerir. Örneğin, "Müdür", "Uzman" gibi unvanlar içerebilir. |
| TitleOfCourtesy | Bu sütun, çalışanın unvanının ne şekilde kullanılması gerektiğini belirtir. Örneğin, "Sayın", "Bay" gibi hödük bir ifade içerebilir. |
| BirthDate       | Bu sütun, çalışanın doğum tarihini içerir. |
| HireDate        | Bu sütun, çalışanın işe alındığı tarihi içerir. |
| Address         | Bu sütun, çalışanın adresini içerir. İşyeri veya ev adresi gibi fiziksel konum bilgilerini içerir. |
| City            | Bu sütun, çalışanın bulunduğu şehri içerir. |
| Region          | Bu sütun, çalışanın bulunduğu bölgeyi içerebilir. Örneğin, eyalet veya ilçe bilgisini içerebilir. |
| PostalCode      | Bu sütun, çalışanın posta kodunu içerir. Posta kodu, coğrafi konumu belirlemek için kullanılır. |
| Country         | Bu sütun, çalışanın bulunduğu ülkeyi içerir. |
| HomePhone       | Bu sütun, çalışanın ev telefon numarasını içerir. |
| Extension       | Bu sütun, çalışanın telefon uzantısını içerebilir. |
| Photo           | Bu sütun, çalışanın fotoğrafını içerebilir. Genellikle bir resim verisi veya resim bağlantısı içerir. |
| Notes           | Bu sütun, çalışanla ilgili notları içerebilir. Özel bilgiler veya notlar burada saklanabilir. |
| ReportsTo       | Bu sütun, çalışanın rapor verdiği kişinin EmployeeID'sini içerebilir. İlgili çalışanın hangi üst düzey çalışana rapor verdiğini belirtir. |
| PhotoPath       | Bu sütun, çalışanın fotoğrafının yolunu içerebilir. Fotoğrafın yerini belirtmek için kullanılır. |
---------------------------------

* **Tablo Adı: EMPLOYEE_TERRITORIES**

| Sütunlar   | Açıklama                                                                                      |
| ---------- | --------------------------------------------------------------------------------------------- |
| EmployeeID | Bu sütun, çalışanın kimlik numarasını içerir ve "EMPLOYEES" tablosundaki ilgili çalışanın kimlik numarasına bir referans sağlar. Bu, ilişkilendirme yapmak için kullanılır. |
| TerritoryID| Bu sütun, çalışanın sorumlu olduğu bölge veya bölgeyi tanımlayan bir kimlik numarasını içerir. Bu, çalışanın atanmış olduğu bölgeleri belirlemek için kullanılır. |
---------------------------------

* **Tablo Adı: ORDER DETAILS**

| Sütunlar   | Açıklama                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------- |
| OrderID    | Bu sütun, siparişleri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır ve sipariş bilgilerini diğer tablolarla ilişkilendirmek için kullanılır. |
| ProductID  | Bu sütun, sipariş edilen ürünü benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır ve ürün bilgilerini diğer tablolarla ilişkilendirmek için kullanılır. |
| UnitPrice  | Bu sütun, her bir ürün biriminin fiyatını içerir. Genellikle para birimi cinsinden tutarları içerir. |
| Quantity   | Bu sütun, her bir ürünün sipariş edilen miktarını içerir. Ürünün kaç birimini sipariş edildiğini belirtir. |
| Discount   | Bu sütun, sipariş edilen ürünün indirim oranını içerir. İndirimli bir fiyat uygulanmışsa, indirim oranını yüzde olarak belirtir. |
---------------------------------

* **Tablo Adı: ORDERS**

| Sütunlar         | Açıklama                                                                                           |
| ---------------- | -------------------------------------------------------------------------------------------------- |
| OrderID          | Bu sütun, siparişleri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| CustomerID       | Bu sütun, siparişi veren müşterinin kimlik numarasını içerir ve "CUSTOMERS" tablosundaki ilgili müşteriye bir referans sağlar. |
| EmployeeID       | Bu sütun, siparişi işleyen veya atanmış olan çalışanın kimlik numarasını içerir ve "EMPLOYEES" tablosundaki ilgili çalışana bir referans sağlar. |
| OrderDate        | Bu sütun, siparişin oluşturulduğu tarihi içerir. |
| RequiredDate     | Bu sütun, siparişin müşteri tarafından istenilen tarihi içerir. Siparişin ne zaman teslim edilmesi gerektiğini belirtir. |
| ShippedDate      | Bu sütun, siparişin gönderildiği tarihi içerir. Siparişin ne zaman sevk edildiğini gösterir. |
| ShipVia          | Bu sütun, siparişin nasıl gönderileceğini belirten bir kimlik numarasını içerebilir. Örneğin, taşıma şirketini tanımlar. |
| Freight          | Bu sütun, nakliye ücretini içerir. Siparişin taşınma maliyetini gösterir. |
| ShipName         | Bu sütun, siparişin teslim edileceği kişinin veya kuruluşun adını içerir. |
| ShipAddress      | Bu sütun, teslimat adresini içerir. |
| ShipCity         | Bu sütun, teslimat şehri veya bölgesini içerir. |
| ShipRegion       | Bu sütun, teslimat bölgesini içerebilir. Örneğin, eyalet veya ilçe bilgisini içerebilir. |
| ShipPostalCode   | Bu sütun, teslimatın posta kodunu içerir. |
| ShipCountry      | Bu sütun, teslimat ülkesini içerir. |
---------------------------------

* **Tablo Adı: PRODUCTS**

| Sütunlar         | Açıklama                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------- |
| ProductID        | Bu sütun, ürünleri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| ProductName      | Bu sütun, ürünün adını içerir. Örneğin, "Laptop", "Çamaşır Makinesi" gibi ürün adları içerebilir. |
| SupplierID       | Bu sütun, ürünü tedarik eden tedarikçinin kimlik numarasını içerir ve "SUPPLIERS" tablosundaki ilgili tedarikçiye bir referans sağlar. |
| CategoryID       | Bu sütun, ürünün hangi kategoriye ait olduğunu belirten bir kimlik numarasını içerir ve "CATEGORIES" tablosundaki ilgili kategoriye bir referans sağlar. |
| QuantityPerUnit  | Bu sütun, birim başına ürün miktarını ve tipini içerir. Örneğin, "10 adet kutu" veya "1 litre şişe" gibi bilgiler içerebilir. |
| UnitPrice        | Bu sütun, bir ürün biriminin fiyatını içerir. Genellikle para birimi cinsinden tutarları içerir. |
| UnitsInStock     | Bu sütun, depoda bulunan ürün birimlerinin sayısını içerir. |
| UnitsOnOrder     | Bu sütun, henüz teslim alınmamış sipariş edilen ürün birimlerinin sayısını içerir. |
| ReorderLevel     | Bu sütun, ürünün yeniden sipariş edilmesi gereken seviyeyi belirten bir değeri içerir. Stok seviyesi bu seviyenin altına düştüğünde yeniden sipariş verilir. |
| Discontinued     | Bu sütun, ürünün devre dışı bırakılıp bırakılmadığını belirten bir bayrak (flag) değerini içerebilir. "1" değeri ürünün devre dışı bırakıldığını, "0" değeri ise devre dışı bırakılmadığını gösterir. |
---------------------------------

* **Tablo Adı: REGION**

| Sütunlar         | Açıklama                                                                                        |
| ---------------- | ----------------------------------------------------------------------------------------------- |
| RegionID         | Bu sütun, bölgeleri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| RegionDescription| Bu sütun, bölgenin açıklamasını içerir. Örneğin, "Kuzey", "Güney", "Batı" gibi bölge adları veya tanımları içerebilir. |
---------------------------------

* **Tablo Adı: SHIPPERS**

| Sütunlar    | Açıklama                                                                                       |
| ----------- | ---------------------------------------------------------------------------------------------- |
| ShipperID   | Bu sütun, taşıma şirketlerini benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| CompanyName| Bu sütun, taşıma şirketinin adını içerir. Örneğin, "Speedy Shipping", "Express Logistics" gibi taşıma şirketi adları içerebilir. |
| Phone       | Bu sütun, taşıma şirketinin iletişim telefon numarasını içerir. Müşterilerin taşıma şirketiyle iletişim kurmak için kullanılabilir. |
---------------------------------
* **Tablo Adı: SUPPLIERS**

| Sütunlar       | Açıklama                                                                                     |
| -------------- | -------------------------------------------------------------------------------------------- |
| SupplierID     | Bu sütun, tedarikçileri benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| CompanyName    | Bu sütun, tedarikçinin şirketinin adını içerir. Örneğin, "ABC Tedarik", "XYZ Şirketi" gibi şirket isimleri içerebilir. |
| ContactName    | Bu sütun, tedarikçi ile iletişim kurulacak kişinin adını içerir. Bu kişi genellikle şirketin temsilcisi olabilir. |
| ContactTitle   | Bu sütun, iletişim kişisinin unvanını içerir. Örneğin, "Satış Müdürü", "CEO" gibi unvanlar içerebilir. |
| Address        | Bu sütun, tedarikçinin adresini içerir. İşyeri veya ev adresi gibi fiziksel konum bilgilerini içerir. |
| City           | Bu sütun, tedarikçinin bulunduğu şehri içerir. |
| Region         | Bu sütun, tedarikçinin bulunduğu bölgeyi içerebilir. Örneğin, eyalet veya ilçe bilgisini içerebilir. |
| PostalCode     | Bu sütun, tedarikçinin posta kodunu içerir. Posta kodu, coğrafi konumu belirlemek için kullanılır. |
| Country        | Bu sütun, tedarikçinin bulunduğu ülkeyi içerir. |
| Phone          | Bu sütun, tedarikçinin telefon numarasını içerir. İletişim için kullanılır. |
| Fax            | Bu sütun, tedarikçinin faks numarasını içerebilir. İhtiyaç halinde iletişim için kullanılır. |
| HomePage       | Bu sütun, tedarikçinin web sitesi veya ana sayfasının bağlantısını içerebilir. |
---------------------------------
* **Tablo Adı: TERRITORIES**

| Sütunlar            | Açıklama                                                                                   |
| ------------------- | ------------------------------------------------------------------------------------------ |
| TerritoryID          | Bu sütun, bölgeleri (territory) benzersiz bir şekilde tanımlayan bir kimlik numarasını içerir. Genellikle birincil anahtar olarak kullanılır. |
| TerritoryDescription | Bu sütun, bölgenin açıklamasını içerir. Örneğin, "Kuzey Bölgesi", "Güneydoğu Bölgesi" gibi bölge adları veya tanımları içerebilir. |
| RegionID             | Bu sütun, bölgenin ait olduğu bölgeyi belirten bir kimlik numarasını içerir. "REGION" tablosundaki ilgili bölgeye bir referans sağlar. |
---------------------------------

## 📌**Veri Seti Tablo İlişkileri ve PostgreSQL ERD :**

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



**NOT :**
* Bu proje ile birlikte e-ticaret verilerinde veri analistinden beklenen görevlerin ve bunlardan alınan sonuçların görselleştirilmesinin ve sunulması gerektiğinin ne kadar önemli olduğunu farkettim. Bu proje ile öğrendğim şeyler kendime yeni bilgiler katmama da çok yardımcı oldu.
* Bu projeyi başarıyla tamamlamamda yardımcı olan herkese teşekkür etmek isterim. Ayrıca, herhangi bir geri bildiriminiz veya öneriniz varsa, lütfen çekinmeden paylaşın. Bu, gelecekteki çalışmalarımızı daha da iyileştirmemize yardımcı olacaktır.
Son olarak ⭐ vermeyi unutmayın, Teşekkürler.
