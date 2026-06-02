# Level 8

## Görev
`data.txt` dosyasında sadece bir kez geçen satırı bul.

## Çözüm
```bash
sort data.txt | uniq -u
```

## Öğrendiklerim
- `sort` satırları sıralar, aynı olanları yan yana getirir
- `uniq -u` sadece bir kez geçen satırları gösterir
- `|` (pipe) bir komutun çıktısını diğerine gönderir
- SOC çalışmasında log analizinde pipe çok kullanılır

## Sonuç
Şifre başarıyla bulundu ve Level 9'a geçildi.
