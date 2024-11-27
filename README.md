# Android Maps API Project

Proyek ini adalah aplikasi Android yang menggunakan Google Maps API untuk menampilkan peta interaktif. Aplikasi ini menyediakan fitur-fitur seperti menampilkan lokasi pengguna, menambahkan marker, dan interaksi dasar dengan peta.

## Fitur Utama
- **Peta Interaktif:** Menampilkan peta menggunakan Google Maps API.  
- **Lokasi Pengguna:** Menampilkan lokasi pengguna di peta (dengan izin lokasi).  
- **Marker Custom:** Menambahkan marker pada lokasi tertentu.  
- **Jenis Peta:** Mendukung berbagai tipe peta (Normal, Satellite, Terrain, dan Hybrid).  

## Teknologi yang Digunakan
- **Bahasa Pemrograman:** Java/Kotlin  
- **IDE:** Android Studio  
- **API:** Google Maps API  

## Prasyarat
1. Android Studio terbaru (versi apa saja yang kompatibel dengan proyek).  
2. Kunci API Google Maps.  
3. Android Studio JAVA/KOTLIN 

## Cara Menggunakan
1. **Clone repositori:**
   ```bash
   git clone https://github.com/SubkhanM/maps-api-project.git
   cd maps-api-project
   ```
2. **Tambahkan kunci API Google Maps:**  
   - Buat kunci API di [Google Cloud Console](https://console.cloud.google.com/).  
   - Tambahkan kunci API Anda ke file `google_maps_api.xml`:
     ```xml
     <string name="google_maps_key">YOUR_API_KEY</string>
     ```
3. **Jalankan aplikasi:**  
   - Buka proyek di Android Studio.  
   - Jalankan di emulator atau perangkat fisik.  

## Struktur Folder
```
maps-api-project/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/maps/
│   │   │   │   └── MainActivity.java
│   │   │   ├── res/
│   │   │   │   └── layout/
│   │   │   │       └── activity_main.xml
│   │   ├── AndroidManifest.xml
│   └── build.gradle
└── README.md
```

## Cuplikan Kode Utama
**Menambahkan Marker di Lokasi Tertentu:**  
```java
LatLng lokasi = new LatLng(-6.200000, 106.816666);
mMap.addMarker(new MarkerOptions().position(lokasi).title("Marker di Jakarta"));
mMap.moveCamera(CameraUpdateFactory.newLatLngZoom(lokasi, 15));
```

## Kontributor
- [Nama Anda](https://github.com/SubkhanM)  

## Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).  
