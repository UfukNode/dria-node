# Dria Node Kurulum Rehberi:

Bu rehberde, GPU destekli cihazlar üzerinden Dria Node'unu Windows veya Linux sistemlerde nasıl kurabileceğinizi adım adım anlattım. Teknik bilginiz olmasa bile rahatça uygulayabilirsiniz.

---

## Neler Yapacağız?

* Windows kurulumu
* Linux kurulumu
* Model seçimi
* Referans kodu girişi ve alma

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

## 5. Model Seçim Önerileri

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

Rehberin videolu versiyonuna @ufukdegen X hesabımdan ulaşabilirsiniz.
