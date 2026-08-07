# Tüm Yollar Roma'ya Çıkar — Three.js MVP

Three.js/WebGL ile hazırlanan masa oyunu prototipi.

## Ana test kuralları

- Tur başında el 7 karta tamamlanır.
- Tur başına en fazla 3 kart oynanır.
- Turu kapatmak için 1 kart ıskartaya atılır.
- Yol kartları masaya konunca kalıcıdır.
- Bir asker yalnızca iki ucu Kale, Ana Kale veya Roma ile tamamlanmış yol segmentlerinde hareket edebilir.
- Kale kartı yeni kale kurmak veya mevcut kalenin seviyesini artırmak için kullanılır.
- Her kale seviyesi +1 savunma ve +3 asker kapasitesi verir.
- Kale seviyesinde yapay üst limit yoktur; toplam Kale kartı sayısı doğal limittir.
- Ele geçirilen kale seviyesini korur.
- Botlar geçerli hamleler arasından basit/rastgele seçim yapar.

## Kontroller

- Kartı elden tahtaya sürükleyip bırak.
- Lejyon grubunu bağlı komşu karta sürükleyerek hareket ettir.
- Sol sürükleme: 3D kamera döndürme.
- Sağ sürükleme: pan.
- Mouse wheel / pinch: zoom.

## Çalıştırma

Yerelde:

```bash
python3 -m http.server 8080
```

Sonra `http://localhost:8080` adresini aç.

GitHub Pages için repo kök dizini yayınlanabilir.
