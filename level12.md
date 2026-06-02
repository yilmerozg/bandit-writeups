# Level 12

## Görev
`data.txt` bir hexdump dosyası, defalarca sıkıştırılmış. Katmanları soyarak şifreyi bul.

## Çözüm
```bash
mktemp -d                    # geçici çalışma klasörü oluştur
cp data.txt /tmp/tmp.xxx/    # dosyayı kopyala
cd /tmp/tmp.xxx/

xxd -r data.txt > data       # hexdump'ı binary'ye çevir
file data                    # her adımda dosya türünü kontrol et

# gzip → bzip2 → tar → tar → bzip2 → tar → gzip katmanları
mv data data.gz && gzip -d data.gz
tar xf data2
tar xf data5.bin
bzip2 -d data6.bin
tar xf data6.bin.out
mv data8.bin data8.gz && gzip -d data8.gz
cat data8
```

## Öğrendiklerim
- `xxd -r` hexdump'ı binary dosyaya çevirir
- `file` komutu her adımda dosya türünü söyler
- `gzip -d` gzip açar, `bzip2 -d` bzip2 açar, `tar xf` tar açar
- Malware analistleri şüpheli dosyaları tam bu şekilde katman katman açar

## Sonuç
Şifre başarıyla bulundu ve Level 13'e geçildi.
