# 🔍 GitHub Unfollow Tool

Seni takip etmeyen GitHub kullanıcılarını tespit et ve tek tıkla takipten çık.

**Sunucu yok, kurulum yok** — sadece `index.html` dosyasını tarayıcında aç ve kullan.

![Dark Theme](https://img.shields.io/badge/theme-dark-0d1117)
![No Server](https://img.shields.io/badge/server-none-success)
![License MIT](https://img.shields.io/badge/license-MIT-blue)

---

## ✨ Özellikler

- 🔑 GitHub Personal Access Token ile giriş
- 📊 Takipçi / Takip edilen / Seni takip etmeyen sayıları
- 🔍 Kullanıcı arama ve filtreleme
- ☑️ Tümünü seç / tekli seçim
- 🚀 Toplu unfollow (rate limit korumalı)
- 📈 İlerleme çubuğu ve işlem özeti
- 🌙 GitHub tarzı koyu tema
- 📱 Mobil uyumlu tasarım

---

## 🚀 Nasıl Kullanılır

### 1. Projeyi İndir

```bash
git clone https://github.com/YOUR_USERNAME/gh-unfollow.git
cd gh-unfollow
```

Ya da direkt olarak `index.html` dosyasını indirin.

### 2. GitHub Token Oluştur

1. [Bu linke tıklayın](https://github.com/settings/tokens/new?scopes=user:follow&description=gh-unfollow) (GitHub Token oluşturma sayfası)
2. Gerekli scope: **`user:follow`**
3. "Generate token" butonuna tıklayın
4. Token'ı kopyalayın

### 3. Kullan

1. `index.html` dosyasını tarayıcınızda açın
2. Token'ınızı girin ve **Bağlan** butonuna tıklayın
3. **Listeyi Yükle** ile seni takip etmeyenleri görün
4. İstediğiniz kullanıcıları seçin
5. **Seçilenleri Unfollow Et** butonuna tıklayın

---

## 🔒 Güvenlik

| Konu | Detay |
|------|-------|
| Token depolama | Sadece tarayıcınızın `localStorage`'ında saklanır |
| Sunucu iletişimi | **Hiçbir sunucuya gönderilmez** — sadece `api.github.com` ile iletişim |
| Kaynak kodu | Tüm kod `index.html` içinde, açık ve okunabilir |
| Çıkış | "Çıkış" butonu token'ı `localStorage`'dan siler |

> ⚠️ **Önemli:** Token'ınızı kimseyle paylaşmayın. Bu uygulama token'ınızı yalnızca GitHub API isteklerinde kullanır.

---

## ⏱ GitHub API Rate Limit

- GitHub API saatte **5.000 istek** hakkı verir (authenticated)
- Her unfollow işlemi arasında **300ms** bekleme süresi uygulanır
- Rate limit **10'un altına** düşünce uyarı verilir
- Rate limit aşılırsa işlem otomatik olarak durur

---

## 🤝 Katkıda Bulunma

1. Bu repoyu fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -m 'feat: yeni özellik'`)
4. Branch'inizi push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request açın

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.
