# Yeni Başlayanlar İçin 10 Temel Shell Komutu

> Bu komutlar hem Linux/macOS terminalinde (bash/zsh) hem de Windows PowerShell'de çalışır.
> PowerShell'de farklı davranan yerler ayrıca not edildi.

---

## 1. `pwd`
**Ne yapar:** Şu an hangi klasörde olduğunu gösterir (print working directory).

**Ne zaman kullanırsın:** Terminali açtın, birkaç kez `cd` yaptın ve nerede olduğunu unuttun. Bir dosyayı kaydetmeden önce doğru klasörde olduğundan emin olmak istiyorsun.
```sh
pwd
# C:\Users\barut\Projeler\website
```

---

## 2. `ls`
**Ne yapar:** Bulunduğun klasördeki dosya ve klasörleri listeler.

**Ne zaman kullanırsın:** İndirdiğin bir projeye girdin ve içinde neler olduğunu (README var mı, hangi klasörler var) görmek istiyorsun.
```sh
ls
ls Downloads        # başka bir klasörün içini listele
```
*PowerShell notu:* Gizli dosyaları görmek için `ls -Force`; bash'te `ls -la`.

---

## 3. `cd`
**Ne yapar:** Başka bir klasöre geçer (change directory).

**Ne zaman kullanırsın:** Masaüstündeki proje klasörüne girip orada çalışmak istiyorsun.
```sh
cd Desktop/proje    # klasöre gir
cd ..               # bir üst klasöre çık
cd ~                # ev klasörüne dön
```

---

## 4. `mkdir`
**Ne yapar:** Yeni bir klasör oluşturur (make directory).

**Ne zaman kullanırsın:** Yeni bir proje başlatıyorsun ve dosyalarını koyacağın bir klasöre ihtiyacın var.
```sh
mkdir yeni-proje
cd yeni-proje
```

---

## 5. `cat`
**Ne yapar:** Bir dosyanın içeriğini terminale yazdırır.

**Ne zaman kullanırsın:** Bir editör açmadan bir ayar dosyasının ya da notun içinde ne yazdığına hızlıca bakmak istiyorsun.
```sh
cat notlar.txt
cat .gitignore
```

---

## 6. `cp`
**Ne yapar:** Bir dosyayı veya klasörü kopyalar (copy).

**Ne zaman kullanırsın:** Önemli bir dosyayı değiştirmeden önce yedeğini almak istiyorsun.
```sh
cp ayarlar.json ayarlar.yedek.json
cp -r fotograflar fotograflar-yedek    # klasörü içindekilerle birlikte kopyala
```

---

## 7. `mv`
**Ne yapar:** Bir dosyayı taşır veya yeniden adlandırır (move).

**Ne zaman kullanırsın:** İndirilenler klasöründeki bir PDF'i ilgili klasöre taşımak ya da `final_son_v3.docx` gibi bir dosyaya düzgün bir isim vermek istiyorsun.
```sh
mv rapor.pdf Belgeler/
mv final_son_v3.docx tez.docx       # yeniden adlandırma
```

---

## 8. `rm`
**Ne yapar:** Dosya veya klasörü siler (remove).

**Ne zaman kullanırsın:** Artık işine yaramayan geçici bir dosyayı ya da eski bir test klasörünü temizlemek istiyorsun.
```sh
rm eski-not.txt
rm -r test-klasoru     # klasörü içindekilerle birlikte sil
```
⚠️ **Dikkat:** `rm` ile silinen dosyalar Çöp Kutusu'na gitmez, geri getirilemez. Çalıştırmadan önce ne sildiğini iki kez kontrol et.

---

## 9. `echo`
**Ne yapar:** Verdiğin metni ekrana yazar; `>` ile bir dosyaya da yazdırabilirsin.

**Ne zaman kullanırsın:** Hızlıca bir dosyaya tek satırlık bir not eklemek ya da bir değişkenin değerini kontrol etmek istiyorsun.
```sh
echo "Merhaba dünya"
echo "toplantı saat 3'te" > hatirlatma.txt    # dosyaya yaz (üzerine yazar)
echo "dosyalari getir" >> hatirlatma.txt      # dosyanın sonuna ekle
```

---

## 10. `clear`
**Ne yapar:** Terminal ekranını temizler.

**Ne zaman kullanırsın:** Ekran uzun çıktılar ve hata mesajlarıyla doldu, temiz bir sayfayla devam etmek istiyorsun. (Kısayol: çoğu terminalde `Ctrl + L`.)
```sh
clear
```

---

## Bonus İpuçları
- **Tab tuşu:** Dosya/klasör adının ilk birkaç harfini yaz, `Tab`'a bas; gerisini otomatik tamamlar.
- **Yukarı ok (↑):** Daha önce yazdığın komutları geri getirir.
- **Ctrl + C:** Takılan veya uzun süren bir komutu durdurur.
- **Yardım almak:** `man ls` (Linux/macOS) veya `Get-Help ls` (PowerShell) bir komutun tüm seçeneklerini gösterir.
