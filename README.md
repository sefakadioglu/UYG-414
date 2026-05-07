# 🧠 AI Intelligent Note Pro
**Bilişsel Analiz ve Mikroservis Tabanlı Akıllı Not Ekosistemi**

Bu proje, geleneksel not alma süreçlerini yapay zeka ile birleştirerek kullanıcıların bilişsel yüklerini yönetmelerine yardımcı olan bir mikroservis ekosistemidir. Proje; **Authentication Gateway**, **Note Service** ve **Notification Service** olmak üzere üç ana modülden oluşmaktadır.

---

## 🛡️ Authentication Gateway (Sefa Cabir Kadıoğlu)
Bu modül, sistemin güvenlik kalkanı ve giriş kapısıdır. Tüm sistem trafiği bu gateway üzerinden doğrulanarak ilgili mikroservislere yönlendirilir.

### 🚀 Kullanılan Teknolojiler
* **Backend:** Python (FastAPI)
* **Veritabanı:** PostgreSQL (Docker konteyner üzerinde izole)
* **Veri Yönetimi:** PGAdmin 4
* **Konteynerizasyon:** Docker & Docker Compose
* **Frontend:** HTML5 & CSS3 (Glassmorphism Tasarım)

### 📸 Geliştirme Süreci ve Görseller

#### 1. Giriş Arayüzü (Kawien AI)
Kullanıcıların sisteme eriştiği ilk noktadır. Minimalist ve modern bir tasarımla, sadece yetkili admin girişine izin verecek şekilde kodlanmıştır.

<img width="1913" height="829" alt="Ekran görüntüsü 2026-05-06 154553" src="https://github.com/user-attachments/assets/9d45ae76-1280-4388-9d4e-862baa36bd71" />

#### 2. Veritabanı ve Docker Entegrasyonu
Sistemde güvenlik verileri için PostgreSQL kullanılmıştır. Docker üzerinde koşan veritabanı, PGAdmin ile birbirine bağlanarak yönetilmektedir. Bu sayede veriler sistemden izole ve güvenli tutulur.

<img width="945" height="1005" alt="image" src="https://github.com/user-attachments/assets/88ea46c1-0a6f-4f6d-af09-655450c438fe" />


#### 3. Proje ve Kod Yapısı
Proje, "Clean Architecture" prensiplerine uygun olarak klasörlenmiştir. `/gateway` klasörü altında tüm doğrulama mantığı ve Docker yapılandırması bulunmaktadır.

<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/9209f370-075e-405d-8ccf-57ad176b6240" />

---

## 🤖 Yapay Zeka ve Akıllı Analiz Sistemi
Sistem, sıradan bir not uygulamasının ötesine geçerek şu özellikleri sunar:

* **Bilişsel Analiz:** Notların içeriğine göre kullanıcının sağ/sol beyin kullanım dengesini ölçer.
* **L1-L4 Önceliklendirme:** Notları önem sırasına göre otomatik olarak sıralar.
* **Vitamin ve Egzersiz Önerileri:** Kullanıcının zihinsel performansını artırmak için Omega-3, B12 gibi takviyeler ve odaklanma egzersizleri önerir.
* **E-Posta Entegrasyonu:** Önemli notları ve yapay zeka özetlerini mail yoluyla paylaşmanızı sağlar.

<img width="1911" height="915" alt="585736948-aea5529c-118a-43f2-9dc4-f537013cb394" src="https://github.com/user-attachments/assets/b795e91d-3c47-434e-87b3-d20c3bad711d" />
<img width="1642" height="906" alt="585737462-05d8859b-5489-42a8-ab5b-63e7aedfc01d" src="https://github.com/user-attachments/assets/cf3fb335-3a2b-402a-a2d2-1a5e0d839946" />


---

## 🛠️ Kurulum (Setup)
Sistemi ayağa kaldırmak için ana dizinde terminali açıp şu komutu yazmanız yeterlidir:

```bash

docker-compose up --build
Access the Dashboard:
Open http://localhost/static/index.html in your browser.
