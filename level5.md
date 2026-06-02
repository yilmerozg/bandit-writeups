# Level 5

## Görev
`inhere` klasöründe şu özelliklere sahip dosyayı bul:
- İnsan tarafından okunabilir
- 1033 byte boyutunda
- Çalıştırılamaz

## Çözüm
```bash
find inhere -size 1033c ! -executable
cat inhere/maybehere07/.file2
```

## Öğrendiklerim
- `find` komutu dosya aramak için kullanılır
- `-size 1033c` → tam 1033 byte boyutunda
- `! -executable` → çalıştırılamaz dosyalar
- Birden fazla özelliği aynı anda filtreleyebiliriz
- SOC çalışmasında şüpheli dosyaları bulmak için `find` çok kullanılır

## Sonuç
Şifre başarıyla bulundu ve Level 6'ya geçildi.
