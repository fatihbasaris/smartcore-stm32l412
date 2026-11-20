
Donanım Özellikleri
===================

Genel Tanım
-----------

SmartCore STM32L412 geliştirme kartı,
STMicroelectronics STM32L412KBT6
mikrodenetleyicisi temel alınarak
tasarlanmıştır.

Kart üzerinde güç yönetimi, USB bağlantısı,
SWD programlama arayüzü, kullanıcı kontrolleri
ve çevresel bağlantılar bulunmaktadır.

Mikrodenetleyici
----------------

* Model: STM32L412KBT6
* Üretici: STMicroelectronics
* İşlemci çekirdeği: ARM Cortex-M4
* Çalışma gerilimi: 3.3 V

Güç Yönetimi
------------

Kartın 3.3 V besleme devresinde
RT9080-33GJ5 gerilim regülatörü
kullanılmıştır.

Devre şemasında VIN, VUSB ve V33
besleme hatları bulunmaktadır.

Besleme girişleri ve çalışma koşulları
devre şeması üzerinden incelenmelidir.

USB Bağlantısı
--------------

Kart üzerinde Mini USB konnektörü
bulunmaktadır.

USB veri hatlarının korunması için
USBLC6-2SC6 ESD koruma bileşeni
kullanılmıştır.

Programlama ve Hata Ayıklama
----------------------------

STM32 mikrodenetleyicisinin programlanması
ve hata ayıklanması için SWD arayüzü
bulunmaktadır.

SWD arayüzü, uygun bir ST-LINK
programlayıcı ile kullanılabilir.

Saat Devresi
------------

Kart üzerinde 32.768 kHz kristal
osilatör devresi bulunmaktadır.

Haberleşme Arayüzleri
---------------------

Kartın bağlantı noktalarında aşağıdaki
arayüzlere ait sinyaller bulunmaktadır:

* UART
* SPI
* I2C
* GPIO

Bu sinyallerin fiziksel pin karşılıkları
Pin Bağlantıları bölümünde açıklanacaktır.

Kullanıcı Kontrolleri
---------------------

Kart üzerinde kullanıcı etkileşimi ve
temel test uygulamaları için butonlar
ve LED göstergeler bulunmaktadır.

Devre Şeması
------------

Kartın elektriksel bağlantıları,
bileşenleri ve sinyal isimleri
STM32L412KBT6 devre şemasında
gösterilmektedir.

Devre şemasının PDF dosyası,
dokümantasyona ayrıca eklenecektir.
