# Level 19

## Görev
Setuid binary kullanarak bandit20'nin şifresini oku.

## Çözüm
```bash
ls                                          # bandit20-do dosyasını gör
./bandit20-do cat /etc/bandit_pass/bandit20 # bandit20 yetkisiyle oku
```

## Öğrendiklerim
- Setuid binary başka kullanıcı yetkisiyle komut çalıştırır
- Saldırganlar yanlış yapılandırılmış setuid binary'leri arar
- Buna privilege escalation denir
- SOC ve blue team çalışmasında bu tür dosyalar izlenir

## Sonuç
Şifre başarıyla bulundu ve Level 20'ye geçildi.
