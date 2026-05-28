# Level 3

## Görev
`inhere` klasöründeki gizli dosyayı bul.

## Çözüm
```bash
ls          # inhere klasörünü gör
cd inhere   # klasöre gir
ls -la      # gizli dosyaları da listele
cat ...Hiding-From-You  # dosyayı oku
```

## Öğrendiklerim
- Linux'ta nokta ile başlayan dosyalar gizlidir
- Normal `ls` gizli dosyaları göstermez
- `ls -la` tüm dosyaları gösterir (-l detaylı, -a gizli dosyalar)
- Saldırganlar dosyalarını gizlemek için bu yöntemi kullanır

## Sonuç
Şifre başarıyla bulundu ve Level 4'e geçildi.
