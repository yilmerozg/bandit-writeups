# Level 10

## Görev
`data.txt` base64 ile kodlanmış, çöz ve şifreyi bul.

## Çözüm
```bash
base64 -d data.txt
```

## Öğrendiklerim
- Base64 veriyi metin formatına çeviren bir kodlama yöntemidir
- Şifreleme değildir, kolayca çözülebilir
- `-d` parametresi decode (çözme) anlamına gelir
- SOC çalışmasında saldırganlar komutlarını base64 ile gizler

## Sonuç
Şifre başarıyla bulundu ve Level 11'e geçildi.
