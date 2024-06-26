### Otomatik Okul Zili Programı - Kullanım Kılavuzu
**Amaç:** Belirli zamanlarda otomatik olarak ilgili zili çalmak ve Arduino tabanlı bir sisteme zil sinyali göndermek.

<p align="center">
  <img src="https://github.com/zengeragency/Otomatik-Okul-Zili/assets/62677804/39759396-3398-45b5-be8b-7d9f6c6c0d56" width="300" alt="Okul Zili">
  <img src="https://github.com/zengeragency/Otomatik-Okul-Zili/assets/62677804/bdd0fd97-5a23-477b-9e36-dd20d1c35bdf" width="300" alt="Okul Zili Sistemi">
</p>

#### Kurulum
0. **İndirme:** Arşivi herhangi bir dizine açın.
1. **Başlangıçta Çalıştırma:** Program başlangıçta çalışması için "Shell:Startup" yoluna kısayol eklenmelidir.
2. Arduino kodu "/Resources" dizinin altındadır.
3. **Arduino Bağlantısı:**

| Pin Adı          | Pin Numarası |
|------------------|--------------|
| PIN_OgrenciZili  | 4            |
| PIN_OgretmenZili | 5            |
| PIN_CikisZili    | 6            |
| LED_BUILTIN      | 17           |

Arduino bilgisayara doğru şekilde bağlandığında otomatik olarak çalışacaktır.

#### Program bildirim çubuğunda çalışıyor. Kapatmak için bildirim çubuğundaki ikona sağ tıklayıp "Programı Kapat" seçeneğine basın.

#### Arayüz Kullanımı
- **Zamanlama Ayarları:**
  - Sabahçı ve öğlenci zil saatleri için zamanlayıcıları ayarlayın.
  - Zil türlerini ve ses seviyelerini belirleyin.
  
- **Ses Ayarları:**
  - Hazır zil seslerinden seçim yapın.
  - Dinle butonuyla sesi kontrol edebilir, durdur butonuyla kesebilirsiniz.

#### Günlük Kayıtlar
- Her zil çalındığında ve Arduino bağlantı durumu değiştiğinde otomatik olarak günlük kayıt tutulur. ```Logs``` klasöründe ```day_yyyy-MM-dd.log``` formatında saklanır.
  
#### Dosyalar ve Klasörler
- **BellSchedule.json:** Zamanlama bilgilerini saklar.
- **Sounds klasörü:** Zil ses dosyalarını içerir. İstenilen sesler bu klasöre eklenebilir.
- **Logs klasörü:** Günlük kayıtlarını tutar.
