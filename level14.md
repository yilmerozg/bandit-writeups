# Level 14

## Görev
Mevcut seviyenin şifresini localhost'un 30000 portuna gönder.

## Çözüm
```bash
echo "MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS" | nc localhost 30000
```

## Öğrendiklerim
- `nc` (netcat) ağ üzerinden veri göndermek için kullanılır
- `echo` ile veriyi pipe ile nc'ye gönderdik
- Port numaraları servisleri ayırt eder
- SOC çalışmasında port testi ve bağlantı kontrolü için nc kullanılır

## Sonuç
Şifre başarıyla bulundu ve Level 15'e geçildi.
