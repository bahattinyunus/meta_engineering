# Bölüm III: Yüksek Seviye Yol Haritası ve Ajan Mimarileri

> *"Geleceği tahmin etmenin en iyi yolu, onu inşa etmektir."* — Alan Kay

Bu bölüm, felsefeden pratiğe geçiş köprüsüdür. Meta-Mühendis olmak için hangi somut yetenekleri kazanmalısınız?

## 3.1. Yetkinlik Seti: Pi-Şekilli İnsan (The Pi-Shaped Engineer)

Düz bir mühendis "T" şeklindedir: Bir konuda derin (dikey), diğer konularda sığ (yatay).
Meta-Mühendis "Pi (Π)" şeklindedir: En az iki alanda derin ve bunların üzerini örten geniş bir çatıya sahiptir.

*   **Sol Ayak (Kök Disiplin):** Yazılım, Makine veya Tıp. Burayı terk etmeyin. Somut dünya bilgisi buradadır. AI, domain bilgisini sizden alır.
*   **Sağ Ayak (AI Okuryazarlığı):** Sadece "kullanmak" değil; "yönetmek". LLM'lerin nasıl çalıştığını, vektör uzaylarını, embedding'leri bilmek zorundasınız.
*   **Çatı (Sistem Mimarlığı):** İki ayağı birleştiren yer. Büyük resmi yönetebilme yeteneği.

## 3.2. Prompt Mühendisliğinin Ötesi: İstem Mimarisi (Prompt Architecture)

"Bana bir e-mail yaz" demek Prompt Engineering'dir (ve artık herkes yapabilir).
Meta-Mühendis, **düşünce zincirleri (Chain of Thought)** kurar.

### Tree of Thoughts (Düşünce Ağacı) Yöntemi
Karmaşık bir problemi çözerken AI'ya tek bir cevap verdirilmez.
1.  **Exploration:** AI'ya 3 farklı çözüm yolu ürettir (Dallar).
2.  **Evaluation:** Her yolun artılarını ve eksilerini değerlendirttir.
3.  **Selection:** En iyi yolu seçtir ve detaylandırttır.

Bu süreci manuel yapmazsınız; bunu yapan Python script'leri (orkestratörler) yazarsınız.

## 3.3. Ajan Bazlı İş Akışları (Agentic Workflows)

Geleceğin yazılım mimarisi **Microservices** değil, **Micro-Agents** olacaktır.
Tek bir süper AI yerine, özelleşmiş küçük AI ajanları takımı.

### Örnek Senaryo: Otonom Yazılım Evi
Bir özellik ekleneceği zaman kurduğunuz mimari:
1.  **Product Manager Agent:** Kullanıcı isteğini alır, "User Story" çıkarır.
2.  **Architect Agent:** Story'yi alır, hangi dosyalarda değişiklik gerektiğini ve veri yapısını planlar.
3.  **Software Engineer Agent:** Planı alır ve kodu yazar.
4.  **QA Agent:** Kodu alır, test yazar, hata bulursa Engineer Agent'a geri yollar (Loop).

Siz bu ajanların kodunu yazmazsınız; siz bu **"konuşma protokolünü"** ve **"yetki sınırlarını"** tasarlarsınız.
Araçlar: *LangChain, CrewAI, AutoGen, Microsoft Semantic Kernel.*

## 3.4. Bir Meta-Mühendisin 24 Saati (Vaka Sahneleri)

Teori güzeldir, peki pratikte hayat nasıl geçer?

### 08:30 - Sabah Kahvesi ve "Özet Ajanı"
E-postaları tek tek okumazsınız. Gece çalışan "Summary Agent", size şunları sunar:
*   "GitHub'da 3 PR açıldı, 2'si otomatik testten geçti, 1'inde güvenlik açığı şüphesi var."
*   "AWS faturası beklenen sınırı %5 aştı, anomali tespiti servisi uyarı verdi."
*   "Sektör haberleri: Rakip firma yeni bir model yayınladı."

### 10:00 - Mimari Tasarım (Orkestrasyon)
Yeni bir proje için kod yazmaya başlamazsınız. **Miro** veya **Excalidraw** benzeri bir tuvalde (Canvas) sistemin diyagramını çizersiniz.
AI, çizdiğiniz diyagramı otomatik olarak Terraform koduna ve klasör yapısına dönüştürür.
Siz: "Hayır, veritabanı NoSQL olmalı, şemayı değiştir." dersiniz. AI düzeltir.

### 14:00 - Sorun Giderme (Human-in-the-Loop)
Üretim hattındaki (Production) bir drone arıza yapar. AI sorunu tespit eder ("Pervane motoru aşırı ısındı") ama çözümü bulamaz.
Müdahale edersiniz. Fizik bilginizi konuşturursunuz. Sisteme yeni bir kural eklersiniz: "Rüzgar hızı 50km/s üstündeyse motor devrini %10 düşür."
Bu "bilgi kırıntısı" sisteme kalıcı olarak işlenir. Bir daha aynı hata olmaz.

### 17:00 - Kendini Güncelleme
Akşam, yeni çıkan bir makaleyi okumazsınız. Makaleyi kendi kişisel bilgi tabanınıza (Second Brain) atarsınız. RAG (Retrieval Augmented Generation) sisteminiz, bu yeni bilgiyi eski bilgilerinizle harmanlar.
Yarın bir soru sorduğunuzda, AI bu yeni makaleyi de hesaba katarak cevap verir.

**Sonuç:** Bir gün içinde 0 satır "manuel" kod yazdınız; ama 10.000 satırlık iş ürettiniz.

## 3.5. Stratejik Kariyer Dönüşümü

1.  **Yatırımı Kendinize Yapın:** Ezbere dayalı sertifikaları bırakın. Problem çözme ve adaptasyon yeteneğinizi kanıtlayan projeler üretin.
2.  **Açık Kaynak:** Kendi kapalı dünyanızdan çıkın. Dünyanın en zeki insanlarıyla aynı repolara commit atın.
3.  **Hibrit Projeler:** Sadece yazılım projesi yapmayın. İçinde donanım olan, içinde biyoloji olan, içinde finans olan projeler geliştirin. Sınırları zorlayın.

Meta-Mühendislik bir varış noktası değil, sürekli bir "oluş" (becoming) halidir.
