# 📰 Haber Botu Pro - Automated News Aggregator

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-21759B?style=for-the-badge&logo=wordpress&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)

[🇬🇧 English](#english) | [🇹🇷 Turkce](#turkce)

---

## <a id="english"></a> 🇬🇧 English

**Haber Botu Pro** is an advanced, automated news aggregator that fetches breaking news from NewsAPI and major RSS feeds. It features a dual-core architecture: a Node.js engine for publishing directly to WordPress (`haber.js`) and a Python engine for broadcasting to Telegram channels (`haber.py`).

### 🚀 Key Features
* **Smart Scoring:** Calculates an importance score based on urgent keywords (e.g., earthquake, explosion) and prioritizes critical news.
* **Auto-Categorization:** Automatically detects the news category (tech, economy, sports, etc.) using keyword analysis.
* **WordPress Integration:** Uploads images and publishes articles automatically via the WP REST API.
* **Telegram Broadcasting:** Sends formatted alerts with images, emojis, and hashtags directly to your Telegram group or channel.
* **Duplicate Prevention:** Uses MD5 hashing to ensure the same news is never published twice.

### 🛠️ Installation & Setup

#### 1. WordPress Bot (Node.js)
* Install the **WP REST API** plugin on your WordPress site and generate an API key (Application Password).
* Edit the configuration block in `haber.js` with your WordPress URL, Username, Application Password, and NewsAPI key.
* Run `npm install` to install required packages.
* Start the bot with `node haber.js` (or `node index.js`).

#### 2. Telegram Bot (Python)
* Open `haber.py` and update the `TelegramHaberBotu` config with your `telegramToken`, `chatId`, and `newsApiKey`.
* Run the bot to start broadcasting news automatically at set intervals.

**Author:** OSSIQN Team | [GitHub Profile](https://github.com/ossiqn)

---

## <a id="turkce"></a> 🇹🇷 Turkce

**Haber Botu Pro**, NewsAPI ve cesitli RSS kaynaklarindan son dakika haberlerini toplayan gelismis bir otomasyon sistemidir. Iki farkli altyapiyi destekler: WordPress sitelerine otomatik icerik girmek icin Node.js (`haber.js`) ve Telegram kanallarina anlik bildirim gondermek icin Python (`haber.py`).

### 🚀 One Cikan Ozellikler
* **Akilli Puanlama Sistemi:** Haber metinlerindeki aciliyet bildiren kelimeleri (deprem, vefat vb.) analiz ederek haberlere onem puani verir ve en onemlileri ilk sirada yayinlar.
* **Otomatik Kategori Algilama:** Icerigi tarayarak haberi dogru kategoriye (teknoloji, ekonomi, spor vb.) otomatik atar.
* **Tam Otomatik WordPress:** WP REST API kullanarak haberleri, gorselleriyle birlikte dogrudan sitenize ekler.
* **Telegram Yayin Agi:** Haberleri emojiler ve hashtagler ile formatlayip resimli olarak Telegram kanalinizda paylasir.
* **Tekrar Onleyici (Anti-Duplicate):** MD5 hash algoritmasi kullanarak ayni haberi asla iki kere paylasmaz.

### 🛠️ Kurulum Adimlari

#### 1. WordPress Botu Icin (Node.js)
* WordPress sitenize girip **WP REST API** eklentisini yukleyin ve API anahtari (Uygulama Sifresi) olusturun.
* `haber.js` icerisindeki ayar kisminda `wordpressUrl`, `wpUsername`, `wpAppPassword` ve `newsApiKey` alanlarini kendi bilgilerinizle doldurun.
* Terminalde `npm install` komutunu calistirarak gerekli modulleri yukleyin.
* Botu baslatmak icin `node haber.js` komutunu calistirin.

#### 2. Telegram Botu Icin (Python)
* `haber.py` dosyasini acin ve en alttaki `TelegramHaberBotu` ayarlarina kendi `telegramToken`, `chatId` ve `newsApiKey` bilgilerinizi girin.
* Kodu calistirdiginizda bot belirlediginiz araliklarla haberleri toplayip kanaliniza atmaya baslayacaktir.

**Gelistirici:** OSSIQN Team | [GitHub Profili](https://github.com/ossiqn)
