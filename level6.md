# Level 6

## Görev
Tüm sunucuda şu özelliklere sahip dosyayı bul:
- bandit7 kullanıcısına ait
- bandit6 grubuna ait
- 33 byte boyutunda

## Çözüm
```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

## Öğrendiklerim
- `find /` tüm sunucuda arama yapar
- `-user` ve `-group` ile dosya sahipliğine göre filtreleme yapılır
- `2>/dev/null` hata mesajlarını gizler
- Linux'ta her dosyanın bir sahibi ve grubu vardır
- Permission denied = erişim engellendi

## Sonuç
Şifre başarıyla bulundu ve Level 7'ye geçildi.
