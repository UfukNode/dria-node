# Dria Node Kurulum Rehberi (Linux – Vast.ai 3060 Test Edildi)

Bu rehberde, GPU destekli bir cihaz (örneğin Vast.ai üzerinde RTX 3060) ile Linux sistem üzerinde Dria Node'unu nasıl kuracağınızı adım adım anlattım. Teknik bilginiz olmasa bile rahatça uygulayabilirsiniz.

---

## 1. Kurulum:

Terminali açın ve aşağıdaki komutları sırasıyla girin:

```bash
sudo apt update && sudo apt install screen -y
```
```bash
curl -fsSL https://ollama.com/install.sh | sh
```
```bash
curl -fsSL https://dria.co/launcher | bash
```
```bash
screen -S dria
```
```bash
dkn-compute-launcher start
```

<img width="1173" height="217" alt="image" src="https://github.com/user-attachments/assets/617d23bf-3b89-49c5-9b4e-aeac921101cb" />

---

## 2. Model Seçimi:

* Yön tuşlarıyla listede gezin.
* "Ollama"yı seçip Enter'a bas.
* "llama3.2:1b-instruct-q4\_K\_M" modelini Space ile seçin, Enter'a basın.
* "Go Back"e gelip Enter yapın.
* Tilki cüzdanının Privkey'ini girin, node'u başlatın.

---

## 3. Ekstra Puan İçin Referans Gir:

* Ctrl + C ile node'u durdurun. (Sonra tekrar başlatacağız)
* Aşağıdaki komutu girin:

```bash
dkn-compute-launcher referrals
```

* İkinci seçeneği seçin, Enter'a basın.
* Referans kodunu girin:
  `vuMidURPoWZMZqHLlqW2`

<img width="459" height="141" alt="Ekran görüntüsü 2025-07-25 201411" src="https://github.com/user-attachments/assets/9a9f914c-ec16-4a41-b16a-bf303fb2a4ab" />

---

## 4. Kendi Referans Kodunu Al:

* Aynı komutu tekrar girin:

```bash
dkn-compute-launcher referrals
```

* İlk seçeneği (Get referral code to refer someone) seçin.
* Ekranda çıkan kod senin referans kodundur.
* Paylaşarak ekstra puan kazanabilirsiniz.

<img width="524" height="215" alt="Ekran görüntüsü 2025-07-25 201451" src="https://github.com/user-attachments/assets/b25c621c-d920-427a-89dc-7b1fa8ec8eea" />

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

* [https://dria.co/edge-ai](https://dria.co/edge-ai) bağlantısına git.
* Sağ üstten “Login” butonuna tıkla.
* Node çalıştırdığın cüzdanın Private Key’i ile giriş yap.
* Node durumunu buradan takip edebilirsin.

<img width="1873" height="941" alt="image" src="https://github.com/user-attachments/assets/ab277fa4-6c15-4673-a2c8-451e2e158235" />

---

## 8. Ayarlara Gitmek İçin

Farklı cüzdandan çalıştırmak veya modeli değiştirmek için:

```bash
dkn-compute-launcher settings
```

<img width="455" height="138" alt="image" src="https://github.com/user-attachments/assets/97cd7501-6e2a-4b0a-94b7-64a921671a6d" />

---

## 9. Dria'yı Tamamen Kaldırmak İçin:

```bash
dkn-compute-launcher uninstall
```

---

**Videolu anlatım için:**
@ufukdegen X hesabım üzerinden videolu rehbere ulaşabilirsiniz.
