# Level 4

## Görev
`inhere` klasöründeki tek insan tarafından okunabilir dosyayı bul.

## Çözüm
```bash
cd inhere     # klasöre gir
file ./*      # tüm dosyaların türünü kontrol et
cat ./-file07 # ASCII text olan dosyayı oku
```

## Öğrendiklerim
- `file` komutu dosyanın içeriğinin türünü söyler
- `ASCII text` = insan tarafından okunabilir metin
- `data` = binary, makine verisi
- `./*` = klasördeki tüm dosyalara uygula
- SOC çalışmasında şüpheli dosyaları analiz ederken `file` komutu çok kullanılır

## Sonuç
Şifre başarıyla bulundu ve Level 5'e geçildi.
