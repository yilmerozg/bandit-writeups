# Level 20

## Görev
`suconnect` adlı setuid binary belirtilen porta bağlanır, oradan okuduğu satırı Level 20 şifresiyle karşılaştırır. Doğruysa Level 21 şifresini gönderir.

## Çözüm
İki terminal sekmesi gerekiyor:

**Sekme 1 (sunucu/dinleyici):**
```bash
nc -l -p 54321
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO   # elle yazıp Enter'a bas
```

**Sekme 2 (client):**
```bash
./suconnect 54321
```

Sekme 1'de Level 21'in şifresi gelir.

## Öğrendiklerim
- `suconnect` client gibi davranıyor, biz sunucu rolünü üstlendik
- `nc -l -p PORT` ile dinleyici/sunucu açılır
- Client-server iletişiminde kim bağlanıyor kim dinliyor ayrımı önemli
- İki terminal sekmesiyle paralel işlem yapılabilir

## Sonuç
Şifre başarıyla bulundu ve Level 21'e geçildi.
