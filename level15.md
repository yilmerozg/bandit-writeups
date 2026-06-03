# Level 15

## Görev
Mevcut şifreyi localhost'un 30001 portuna SSL/TLS ile gönder.

## Çözüm
```bash
echo "8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo" | openssl s_client -connect localhost:30001 -quiet
```

## Öğrendiklerim
- `openssl s_client` SSL/TLS şifreli bağlantı kurar
- Normal nc şifresiz, openssl şifreli veri gönderir
- http vs https farkı gibi — https SSL/TLS kullanır
- Self-signed certificate uyarısı normal, sunucu kendi sertifikasını imzalamış
- SOC çalışmasında şifreli ve şifresiz trafik ayrımı kritiktir

## Sonuç
Şifre başarıyla bulundu ve Level 16'ya geçildi.
