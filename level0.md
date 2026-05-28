# Level 0

## Görev
Bandit sunucusuna SSH ile bağlan ve `readme` dosyasındaki şifreyi bul.

## Bağlantı
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
Şifre: `bandit0`

## Çözüm
```bash
ls        # klasördeki dosyaları listele
cat readme  # dosyanın içini oku
```

## Öğrendiklerim
- `ssh` komutu ile uzak sunucuya bağlanılır
- `-p 2220` parametresi port numarasını belirtir
- `ls` komutu dosyaları listeler
- `cat` komutu dosya içeriğini ekrana yazdırır

## Sonuç
Şifre başarıyla bulundu ve Level 1'e geçildi.
