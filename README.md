# 🚗 Yakıt Tüketim Analiz Sistemi


Bu proje; araç kullanıcılarının yolculuk verilerini analiz etmelerini sağlayan, veri görselleştirme (plotting) bileşenleri barındıran ve arka planda **basit lineer regresyon** tahmin modeli kullanan modern bir MATLAB masaüstü arayüz (GUI) uygulamasıdır.

---

## 📌 Öne Çıkan Özellikler
* 📊 **Anlık Grafik Görselleştirme:** Mesafeye göre tüketim trendi ve regresyon tabanlı maliyet öngörüsü.
* 🤖 **Akıllı Tahmin Modeli:** `polyfit` ve `polyval` algoritmaları ile gelecekteki yakıt maliyetlerini dinamik hesaplama.
* 🛡️ **Veri Doğrulama (Data Validation):** Hatalı, eksik veya negatif girişleri engelleyen güvenli mimari.
* 🖥️ **Masaüstü Entegrasyonu:** MATLAB Compiler ile son kullanıcının bilgisayarında MATLAB kurulu olmasa bile çalışabilen standalone `.exe` çıktısı.

---

## 📂 Proje Yapısı ve Dosyalar

| Dosya Adı | Açıklama |
| :--- | :--- |
| `FuelConsumptionAnalysisSystem_App.m` | `uifigure` tabanlı, modern nesne yönelimli ana GUI arayüz sınıfı. |
| `computeFuelConsumption.m` | Doğrulama, metrik hesaplama ve regresyon modellerini içeren çekirdek analiz motoru. |
| `runFuelConsumptionApp.m` | Uygulamayı tek komutla başlatan entegrasyon scripti. |
| `buildStandaloneExe.m` | Projeyi bağımsız bir `.exe` kurulum paketine dönüştüren derleme scripti. |
| `FuelConsumptionAnalysisSystem_Phase1.m` | Projenin ilk fazına ait CLI/Script referans sürümü. |

---

## 🛠️ Sistem Gereksinimleri
* **MATLAB R2026a** veya daha yeni bir sürüm.
* **Core Fonksiyonlar:** Ekstra hiçbir toolbox gerektirmez (Standart `polyfit`, `uitable`, `uiaxes` bileşenleri kullanılmıştır).
* **EXE Üretimi İçin:** Sistemde **MATLAB Compiler** kurulmuş olmalıdır.

---

## 🚀 Çalıştırma Talimatları

Proje klasörünü MATLAB üzerinde açtıktan sonra Komut Penceresine (`Command Window`) aşağıdaki komutu yazarak uygulamayı başlatabilirsiniz:

```matlab
runFuelConsumptionApp