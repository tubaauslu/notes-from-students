# Katki ve Moderasyon Kurallari
## Klasör İsimlendirme Kuralları

Projeye yeni notlar eklerken karmaşayı önlemek için klasör yapısının `Bolum/Sinif/Ders/` şeklinde olmasına dikkat edin. Klasörleri oluştururken şu kurallara uyun:

* **Bölüm Adı:** Türkçe karakter (ç, ş, ğ, ü, ö, ı) kullanılmamalı ve boşluklar yerine alt çizgi (`_`) konulmalıdır. 
  *(Örnek: `Bilgisayar_Muhendisligi`)*
* **Sınıf Adı:** Rakam ve `_Sinif` formatında yazılmalıdır.
  *(Örnek: `1_Sinif`, `2_Sinif`)*
* **Ders Adı:** **Ders kodu** mutlaka kullanılmalı ve ders adı ile arasına alt çizgi (`_`) konulmalıdır. Türkçe karakter kullanılmamalıdır.
  *(Örnek: `BLM101_Programlama`, `BLM201_Veri_Yapilari`)*
  ## 🔍 Moderasyon ve İnceleme Süreci

Gönderdiğiniz Pull Request'ler (PR), repomuzun kalite standartlarını korumak amacıyla bölüm sorumluları tarafından incelenir. Bu süreçte ve genel organizasyonda **YAZGIT organizasyon kurallarına** mutlak suretle uyulması beklenmektedir.

### PR Kabul ve Ret Kriterleri
Eklenen notlar şu kriterlere göre değerlendirilir:
* **Doğruluk:** Notlardaki akademik/teknik bilgilerin büyük hatalar içermemesi.
* **Okunabilirlik:** Taranmış PDF'lerin veya metinlerin düzenli, net ve okunaklı olması.
* **Kurallara Uygunluk:** Klasör ve dosya isimlendirme kurallarına (Türkçe karakter kullanmama, ders kodu belirtme vb.) uyulması.
* **Tamlık:** Eksik sayfa veya yarım kalmış içeriklerin bulunmaması.

### Yapay Zeka (AI) Politikası
Yapay zeka (ChatGPT, Gemini vb.) ile üretilmiş ders özetleri veya notlar gönderilirken, bu durum PR açıklamasında **açıkça belirtilmelidir**. Kontrol edilmemiş ve hatalı (halüsinasyon) bilgiler içeren yapay zeka çıktıları doğrudan reddedilecektir.

### Hedef İnceleme Süresi
Gönderilen PR'lar, ilgili bölümün yetkilileri tarafından aksi bir durum olmadıkça **en geç 3-5 iş günü** içerisinde incelenip sonuçlandırılacaktır.

## ⚠️ İçerik Politikası ve Akademik Dürüstlük

Repomuza eklenecek notlar, telif haklarına ve akademik dürüstlük kurallarına kesinlikle uymalıdır. Sadece kendi tuttuğunuz, derlediğiniz veya açık paylaşım izni olan özgün notları yükleyebilirsiniz.

**Kurallar ve Yasaklı İçerik Örnekleri:**
Aşağıdaki materyallerin repoya eklenmesi **kesinlikle yasaktır**:
* **Hoca Slaytları ve Ders Kitapları:** Hocaların izni olmadan paylaşılan sunumlar (PPTX, PDF) ile telif hakkı ile korunan ders kitaplarının PDF kopyaları veya kitaptan doğrudan kopyalanan/taranan içerikler.
* **Devam Eden Sınavlar:** Henüz süresi dolmamış/tamamlanmamış sınavlara, quizlere veya aktif ödevlere ait materyaller ve çözüm yolları. (Bu durum doğrudan akademik dürüstlük ihlalidir).
* **Geçmiş Sınav Soruları:** Hocanın açıkça paylaşılmasına izin vermediği çıkmış sınav soruları.
* **İzinsiz İçerikler:** Başka öğrencilere ait, izin alınmadan yüklenen ödevler, projeler ve kişisel notlar.

### 🗑️ İçerik Kaldırma Talepleri (Takedown Requests)
Repomuzda yer alan herhangi bir materyalin telif hakkınızı ihlal ettiğini veya izinsiz paylaşıldığını düşünüyorsanız (öğretim görevlileri, öğrenciler veya diğer hak sahipleri), lütfen bizimle iletişime geçin:
* **İletişim Yolu:** GitHub üzerinden durumu anlatan yeni bir **Issue** açabilirsiniz.
* **Sorumlu Kişi ve Hedef Süre:** Kaldırma talepleri, repo yöneticisi (@tubaauslu) tarafından en geç **48 saat (2 iş günü)** içerisinde incelenecek ve ihlal tespit edilmesi durumunda içerik derhal repodan silinecektir.

## 📝 Üst Bilgi (Header) ve Atıf Kuralları

Projeye eklediğiniz notların (özellikle Markdown, Word veya PDF belgelerinin) en üstünde, içeriğin bağlamını belirten kısa bir bilgi bölümü bulunmalıdır.

**Örnek Üst Bilgi Formatı:**
* **Ders:** (Örn: BLM101 Programlama)
* **Dönem:** (Örn: 2023-2024 Güz)
* **Öğretim Üyesi:** (Örn: Prof. Dr. Ad Soyad)
* **Yazar (İsteğe Bağlı):** Gerçek adınızı, takma adınızı (nickname) veya GitHub kullanıcı adınızı yazabilir ya da bu alanı tamamen anonim bırakabilirsiniz.

**Kaynak ve Atıf Kuralı:**
Notlarınızı derlerken ders kitapları, akademik makaleler, web siteleri veya başka öğrencilerin notlarından faydalandıysanız, belgenin sonuna mutlaka bir "Kaynaklar" bölümü eklemelisiniz. Doğrudan alınan metinlerin, kod bloklarının veya görsellerin orijinal kaynağı (kitap adı, sayfa numarası veya URL) açıkça belirtilmelidir.

## 🚀 Katkı İş Akışı (Contribution Workflow)

Projeye yeni notlar eklerken lütfen aşağıdaki adımları ve standartları takip edin:

**1. Fork'u Güncel Tutma**
Çalışmaya başlamadan ve yeni bir dal (branch) açmadan önce, kendi fork'unuzun ana repoyla (upstream) senkronize olduğundan emin olun:
```bash
git fetch upstream
git checkout main
git merge upstream/main## 🚀 Katkı İş Akışı (Contribution Workflow)

2. Dal (Branch) İsimlendirme Kuralları
Dal adları tutarlı olmalı, Türkçe karakter içermemeli ve yapılan işin türünü İngilizce bir ön ek ile belirtmelidir:

Yeni içerik veya not ekleme: feat/ders-adi-notlar (Örn: feat/blm101-vize)

Hata düzeltme (yanlış dosya vb.): fix/dosya-adi-duzeltme

Dokümantasyon güncellemeleri: docs/readme-guncellemesi

3. Commit Mesajı Kuralları
Commit mesajlarınız ne yapıldığını net bir şekilde açıklamalıdır. Mesajın başına yapılan işin türünü ekleyin:

feat: BLM101 programlama vize notları eklendi

fix: klasör ismindeki yazım hatası düzeltildi

docs: CONTRIBUTING dosyasına yeni kurallar eklendi

4. Pull Request (PR) Başlık ve Açıklama Rehberi

Başlık: PR başlığı, eklediğiniz içeriği kısa ve öz bir şekilde özetlemelidir (Örn: feat: Elektrik Devreleri final çalışma soruları).

Açıklama: PR açıklamasında; notların hangi derse, döneme ve öğretim üyesine ait olduğunu belirtin. Notlarda eksik kısımlar veya belirtilmesi gereken özel durumlar varsa bunları mutlaka yazın.