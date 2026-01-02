# so_long

## Proje Hakkında (TR)
Bu proje, 42 eğitim programı kapsamında, MiniLibX grafik kütüphanesi kullanılarak geliştirilmiş 2D bir "toplama ve kaçış" oyunudur. Projenin temel amacı, grafik arayüzü yönetimi, olay döngüleri (event loops) ve harita işleme mantığını kavramaktır.

### Öne Çıkan Özellikler
- **Cross-Platform Desteği**: Makefile ve kaynak kodları hem macOS hem de Linux (Ubuntu/Debian) sistemlerinde sorunsuz çalışacak şekilde optimize edilmiştir.
- **Akıllı Harita Kontrolü**: Haritanın çevrelenmiş duvarlarını ve objelerin (P, E, C) geçerliliğini kontrol eden katı bir validasyon sistemi.
- **Flood Fill Algoritması**: Oyun başlamadan önce çıkışa ve tüm toplanabilir öğelere ulaşılabilir bir yol olup olmadığını kontrol eden algoritma.
- **Esnek Kontrol**: Hem klasik WASD hem de Yön Tuşları desteği.

### Proje Yapısı
- **gnl/**: Get Next Line fonksiyonu (harita okuma için).
- **maps/**: .ber uzantılı örnek harita dosyaları.
- **mlx/**: MiniLibX kütüphanesi.
- **textures/**: Karakter, duvar ve objeler için .xpm görselleri.
- **so_long.h**: Cross-platform tuş kodları ve yapı tanımları.

---

## About the Project (EN)
This project is a 2D "collect-and-escape" game developed using the MiniLibX library as part of the 42 curriculum. The core objectives are to master graphical interface management, event loops, and map parsing logic.

### Key Features
- **Cross-Platform Support**: The Makefile and source code are optimized to run seamlessly on both macOS and Linux systems.
- **Robust Map Validation**: A strict system that verifies map boundaries and the validity of game objects (P, E, C).
- **Flood Fill Algorithm**: Ensures there is a valid path to the exit and all collectables before the game starts.
- **Flexible Controls**: Support for both classic WASD and Arrow Keys.

### Project Structure
- **gnl/**: Get Next Line function (for map parsing).
- **maps/**: Sample map files with the .ber extension.
- **mlx/**: MiniLibX library.
- **textures/**: .xpm assets for the character, walls, and game objects.
- **so_long.h**: Header file containing cross-platform keycodes and structure definitions.

---

## Kurulum ve Çalıştırma / Installation & Usage
1. Derleme (Compilation)
   ```bash
   make
2. Çalıştırma (Running)
   ```bash
   ./so_long maps/map.ber

### Önemli Not / Important Note
Bu repoda bulunan mlx klasörü Linux sistemleri için yapılandırılmıştır. Eğer projeyi macOS üzerinde çalıştırmak isterseniz mevcut mlx klasörünü silip yerine macOS uyumlu MiniLibX sürümünü eklemelisiniz.
The mlx folder in this repository is configured for Linux systems. If you want to run this project on macOS you must replace the current mlx folder with the macOS-compatible version of MiniLibX.
