# Level 17

## Görev
`passwords.old` ve `passwords.new` arasındaki tek farklı satırı bul.

## Çözüm
```bash
diff passwords.old passwords.new
```

## Öğrendiklerim
- `diff` iki dosya arasındaki farkları gösterir
- `<` eski dosyadaki satır, `>` yeni dosyadaki satır
- SOC çalışmasında log veya config dosyalarını karşılaştırmak için kullanılır

## Sonuç
Şifre başarıyla bulundu ve Level 18'e geçildi.
