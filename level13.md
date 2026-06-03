# Level 13

## Görev
Şifre verilmiyor, bunun yerine SSH private key ile bandit14'e bağlan.

## Çözüm
```bash
# bandit13'te key'i görüntüle
cat sshkey.private

# Kali'de key dosyası oluştur
nano ~/sshkey14.private  # key'i yapıştır
chmod 600 ~/sshkey14.private  # izin ver

# Key ile bağlan
ssh -i ~/sshkey14.private bandit14@bandit.labs.overthewire.org -p 2220

# Şifreyi oku
cat /etc/bandit_pass/bandit14
```

## Öğrendiklerim
- SSH key pair: private key sende, public key sunucuda durur
- Şifre yerine key ile bağlanmak daha güvenlidir
- `-i` parametresi key dosyasını belirtir
- `chmod 600` key dosyasını sadece sahibin okuyabileceği şekilde ayarlar
- Gerçek şirket sunucularına SSH key ile bağlanılır

## Sonuç
Şifre başarıyla bulundu ve Level 14'e geçildi.
