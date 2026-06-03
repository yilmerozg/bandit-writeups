# Level 18

## Görev
`.bashrc` değiştirilmiş, bağlanınca otomatik çıkış yapıyor. readme dosyasını oku.

## Çözüm
```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat ~/readme"
```

## Öğrendiklerim
- SSH ile shell açmadan direkt komut çalıştırılabilir
- `.bashrc` her bash oturumunda otomatik çalışır
- Saldırganlar `.bashrc` değiştirerek persistence sağlar
- Bu tür değişiklikleri tespit etmek SOC analistinin görevidir

## Sonuç
Şifre başarıyla bulundu ve Level 19'a geçildi.
