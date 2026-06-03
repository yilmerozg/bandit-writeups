# Level 16

## Görev
31000-32000 arasındaki portları tara, SSL konuşan doğru porta şifreyi gönder.

## Çözüm
```bash
# Açık portları tara
nmap -p 31000-32000 localhost

# Her porta SSL ile dene
echo "kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx" | openssl s_client -connect localhost:31790 -quiet 2>/dev/null
```

## Öğrendiklerim
- `nmap` port tarama aracıdır
- Bazı portlar veriyi geri yansıtır (echo), doğru port credentials döner
- Bu sefer şifre değil SSH private key aldık
- SOC çalışmasında nmap ile açık portları tespit etmek temel beceridir

## Sonuç
SSH private key alındı ve Level 17'ye geçildi.
