# Level 11

## Görev
`data.txt` ROT13 ile şifrelenmiş, çöz ve şifreyi bul.

## Çözüm
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

## Öğrendiklerim
- ROT13 her harfi alfabede 13 pozisyon kaydırır
- `tr` komutu karakter dönüşümü yapar
- SOC çalışmasında saldırganlar basit obfuscation için ROT13 kullanır
- Pipe ile cat ve tr birleştirildi

## Sonuç
Şifre başarıyla bulundu ve Level 12'ye geçildi.
