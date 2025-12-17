# Katkı Protokolü (Contributing.exe)

> *"Geleceği compile etmeye hoş geldiniz."*

Bu repository, statik bir kütüphane değil; sürekli gelişen dinamik bir bilgi tabanıdır (Living Knowledge Base). Sizin katkılarınız (Pull Requests), bu sistemin evriminde kritik birer mutasyon rolü oynar.

## Git Akışı ve Katkı Mimarisi

Bireysel kahramanlıklar yerine, dağıtık ve versiyonlu bir işbirliği modelini benimsiyoruz.

### 1. Fork & Clone
Ana depoda (Main Branch) doğrudan 'write' yetkiniz yoktur. Önce repoyu kendi alanınıza forklayın:
```bash
git clone https://github.com/bahattinyunus/meta.git
```

### 2. Dal Stratejisi (Branching Strategy)
Asla `main` üzerinde çalışmayın. Yaptığınız işe uygun isimlendirilmiş bir dal (branch) açın:

*   **Yeni Özellik/Bölüm:** `feature/bolum-adi` (Örn: `feature/bolum-06-bci`)
*   **Düzeltme:** `fix/hata-tanimi` (Örn: `fix/readme-typo`)
*   **İyileştirme:** `refactor/konu` (Örn: `refactor/kod-bloklari`)

### 3. Commit Düsturları
Commit mesajlarınız gelişi güzel olmamalıdır. "Conventional Commits" standardını takip edin:
*   `feat: Yeni bölüm 4 tasarımı eklendi`
*   `fix: Markdown link hatası giderildi`
*   `docs: README güncellendi`

> *İyi bir commit mesajı, gelecekteki Meta-Mühendislere bırakılmış bir nottur.*

### 4. Pull Request (PR) Süreci
*   Değişikliklerinizi tamamladıktan sonra bir PR açın.
*   PR açıklamanızda **NE** yaptığınızı ve **NEDEN** yaptığınızı detaylandırın.
*   Varsa ilgili "Issue" numarasını referans verin.
*   Code Review sürecinde gelen geri bildirimleri kişisel algılamayın; kodunuzu (veya yazınızı) optimize ediyoruz, sizi değil.

## İçerik Standartları

*   **Dil:** Türkçe (Resmi, teknik ve felsefi terminolojiye uygun).
*   **Format:** Standart Markdown.
*   **Stil:** Kısa paragraflar, net başlıklar. "Wall of text"ten kaçının.

---
*Her commit, entropiye karşı bir zaferdir.*
