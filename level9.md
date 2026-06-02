# Level 9

## Görev
`data.txt` dosyasında `=` işaretlerinden önce gelen okunabilir stringi bul.

## Çözüm
```bash
strings data.txt | grep "=="
```

## Öğrendiklerim
- `strings` binary dosyadan okunabilir metinleri çeker
- `grep "=="` sadece = içeren satırları filtreler
- İki komut pipe ile birleştirildi

## Sonuç
Şifre başarıyla bulundu ve Level 10'a geçildi.
