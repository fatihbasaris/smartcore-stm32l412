
Programlama ve Hata Ayıklama
===========================

Genel Bakış
-----------

SmartCore STM32L412 geliştirme kartı,
STM32CubeIDE geliştirme ortamı kullanılarak
programlanabilir.

Kartın SWD arayüzü üzerinden ST-LINK
programlayıcı ile yazılım yükleme ve
hata ayıklama işlemleri gerçekleştirilebilir.

Gerekli Yazılımlar
------------------

* STM32CubeIDE
* STM32CubeProgrammer
* STM32L4 mikrodenetleyici desteği

Yazılım İndirme Bağlantıları
---------------------------

STM32CubeIDE:

https://www.st.com/en/development-tools/stm32cubeide.html

STM32CubeProgrammer:

https://www.st.com/en/development-tools/stm32cubeprog.html

Donanım Bağlantısı
------------------

Programlama için ST-LINK programlayıcı,
kartın SWD bağlantı noktalarına bağlanır.

Temel SWD sinyalleri:

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Sinyal
     - Açıklama
   * - SWDIO
     - Çift yönlü SWD veri hattı
   * - SWCLK
     - SWD saat hattı
   * - GND
     - Ortak toprak bağlantısı
   * - VTref
     - Hedef sistem gerilim referansı
   * - NRST
     - Reset bağlantısı (isteğe bağlı)

Konnektör pin numaraları için kartın
devre şemasına başvurulmalıdır.

STM32CubeIDE ile Proje Oluşturma
--------------------------------

1. STM32CubeIDE uygulamasını başlatın.

2. File > New > STM32 Project seçeneğini açın.

3. MCU/MPU Selector bölümünde
   STM32L412KBT6 mikrodenetleyicisini seçin.

4. Projeye bir isim verin.

5. Pinout & Configuration ekranında
   SYS > Debug ayarını Serial Wire yapın.

6. Kullanılacak GPIO ve çevresel
   birimleri yapılandırın.

7. Project > Generate Code seçeneğiyle
   gerekli kodları oluşturun.

8. Uygulama kodunu ekleyin ve
   projeyi derleyin.

Yazılım Yükleme
---------------

1. Geliştirme kartını uygun şekilde besleyin.

2. ST-LINK bağlantısını kontrol edin.

3. STM32CubeIDE içerisinde projeyi açın.

4. Run > Debug veya Run > Run
   komutunu kullanın.

5. Programlama tamamlandıktan sonra
   uygulamanın çalışmasını kontrol edin.

Hata Ayıklama
-------------

STM32CubeIDE hata ayıklama araçları ile:

* Breakpoint oluşturulabilir.
* Değişken değerleri izlenebilir.
* Program adım adım çalıştırılabilir.
* Mikrodenetleyici register değerleri
  incelenebilir.

Notlar
------

* SWD bağlantıları doğru yapılmalıdır.
* ST-LINK ve kart ortak GND hattını paylaşmalıdır.
* Hedef kartın besleme gerilimi kontrol edilmelidir.
* VTref hattı, hedef sistemin lojik
  gerilimini algılamak için kullanılır.
* Programlama sırasında uygun
  STM32L412KBT6 hedefi seçilmelidir.
