# Dria Node Kurulum Rehberi (Windows):

Bu rehberde, GPU destekli cihazlar üzerinden Dria Node'unu Windows' nasıl kurabileceğinizi adım adım anlattım. Teknik bilginiz olmasa bile rahatça uygulayabilirsiniz.

---

## GPU Gereksinimi

Eskiden CPU ile çalışan modeller varken, artık yalnızca GPU destekli modeller kullanılabilmektedir. Bu nedenle GPU destekli bir cihaz şarttır.

**Öneri:**
Sanal sunucunuzda veya kendi bilgisayarınızda çalıştırın, ekstra para harcamaya gerek yok.

---

## - 1. Windows Kurulumu

### PowerShell Üzerinden Kurulum

PowerShell'i açın ve aşağıdaki komutları sırayla girin:

```powershell
powershell -c "irm https://dria.co/launcher.ps1 | iex"
```
```powershell
$env:PATH = [System.Environment]::GetEnvironmentVariable("PATH","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("PATH","User")
```
```powershell
dkn-compute-launcher.exe start
```

---

## 2. Model Seçimi

- Yön tuşlarıyla listede gezin.
- "Ollama"yı seçip Enter'a bas.
- "llama3.2:1b-instruct-q4_K_M" modelini Space ile seç, Enter'a bas.
- "Go Back"e gelip Enter yap.
- Tilki cüzdanının Privkey'ini gir, node'u başlat.

---

## 3. Ekstra Puan İçin Referans Girmek

- Ctrl + C ile node'u durdur.
- Aşağıdaki komutu gir:

```powershell
dkn-compute-launcher referrals
```

- İkinci seçeneği seçip Enter yap.
- Referans kodunu gir: vuMidURPoWZMZqHLlqW2

---

## 4. Kendi Referans Kodunu Almak

- Aşağıdaki komutu tekrar girin.

```powershell
dkn-compute-launcher referrals
```

- "Get referral code to refer someone" seçeneğini seç.
- Ekranda çıkan mavi yazılı kod senin referans kodundur.
- Paylaşarak ekstra puan kazanabilirsin.

---

## 5. Discord Rolü

Kurulumu tamamladıktan sonra aşağıdaki formu doldurarak Discord rolünüzü alabilirsiniz, dostlar.

* Form: [https://form.typeform.com/to/Eav42hR3](https://form.typeform.com/to/Eav42hR3?typeform-source=www.google.com)
* Discord: [https://discord.gg/dria](https://discord.gg/dria)

---

## 6. Model Seçim Önerileri

**Sisteminiz Düşükse:**

* llama3.2:1b
* llama3.1:8b
* gemma3:4b

**Güçlü Sistemler İçin:**

* gemma3:12b
* mistral-nemo:12b
* gemma3:27b
* llama3.3:70b

---

## 7. Durumunu Kontrol Et:

- https://dria.co/edge-ai bağlantıya git.
- Sağ üstten login butonuna tıkla.
- Private Keyi ile node çalıştırdığın cüzdan ile giriş yap.
- Durumunu bu şekilde takip edebilirsiniz.


## 8. Dria ayarlara Gitmek İçin:

- Farklı cüzdandan çalıştırmak veya modeli değiştirmek için ayarları buradan yapabilirsiniz.

```powershell
dkn-compute-launcher settings
```

---

## 9. Dria'yı Silmek İçin:

```powershell
Remove-Item -Path "$HOME\Downloads\launcher.ps1", "$HOME\AppData\Local\Temp\launcher.ps1" -Force -ErrorAction SilentlyContinue
```

---

Rehberin videolu versiyonuna @ufukdegen X hesabımdan ulaşabilirsiniz.
