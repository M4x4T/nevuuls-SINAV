
---

### **Frekans Tablosu Oluşturma: Adım Adım Rehber**

İstatistikte frekans, bir verinin **kaç kez tekrarlandığını** gösterir. Örnekde; "Kaç öğrenci Kayserili? Kaç tanesi Nevşehirli?" gibi soruların cevabıdır.

#### **Adım 1: Verileri Gruplandır (Ham Veri)**
Diyelim ki 10 öğrenciye sorduk ve şu cevapları aldık: 
*Kayseri, Nevşehir, Kayseri, Ankara, Nevşehir, Kayseri, Ankara, Kayseri, Nevşehir, Ankara.*

#### **Adım 2: Frekans ($f$) Türlerini Hesapla**


**1. Mutlak Frekans ($f_i$):**
Her bir kategorinin (şehrin) kaç kez tekrarlandığıdır. Sadece sayıyoruz.
* Kayseri: 4 kişi
* Nevşehir: 3 kişi
* Ankara: 3 kişi
* **Toplam ($n$):** 10

**2. Oransal (Göreceli) Frekans ($rf_i$):**
Her bir grubun toplam içindeki payıdır. 1 üzerinden hesaplanır.
* **Formül:** $rf_i = \frac{f_i}{n}$
* Kayseri için: $4 / 10 = 0,40$
* Nevşehir için: $3 / 10 = 0,30$
* Ankara için: $3 / 10 = 0,30$
* *Not: Toplamı her zaman 1,00 olmalıdır.*

**3. Yüzdesel Frekans ($\%$):**
Oransal frekansın 100 ile çarpılmış halidir. Anlaması en kolay olanıdır.
* **Formül:** $rf_i \times 100$
* Kayseri: $\%40$
* Nevşehir: $\%30$
* Ankara: $\%30$
* *Not: Toplamı her zaman 100 olmalıdır.*

**4. Birikimli (Kümülatif) Frekans ($F_i$):**
Frekansların üst üste eklenerek toplanmasıdır. Genellikle sıralı verilerde (azdan çoğa) "bu değere kadar toplam kaç kişi var?" sorusuna yanıt verir.
* Kayseri: 4
* Nevşehir: $4 + 3 = 7$
* Ankara: $7 + 3 = 10$



**5. Birikimli Oransal (Göreceli) Frekans ($BRF$ veya $RF_c$):**
Oransal frekansların ($rf$) üst üste toplanmasıyla elde edilir. Verilerin o kategoriye gelene kadar toplamın kaçta kaçını oluşturduğunu gösterir.
* **Formül:** Bir önceki satırın Birikimli Oransal Frekansı + O satırın Oransal Frekansı.
* **Kritik Bilgi:** Tablonun en son satırındaki değer mutlaka **1,00** olmalıdır.

**6. Birikimli Yüzdelik Frekans ($\%C$):**
Yüzdelik frekansların ($\%$) üst üste toplanmasıdır. "Sınıfın yüzde kaçı bu kategorinin altında kalıyor?" sorusuna yanıt verir.
* **Formül:** Birikimli Oransal Frekans $\times 100$.
* **Kritik Bilgi:** Tablonun en son satırındaki değer mutlaka **100** olmalıdır.


**Özet Tablo Mantığı:**
1.  **Mutlak ($f$):** Say adetleri.
2.  **Birikimli ($F$):** Sayıları toplayarak git.
3.  **Oransal ($rf$):** Adedi toplama böl.
4.  **Birikimli Oransal ($BRF$):** Oranları toplayarak git.
5.  **Yüzde ($\%$):** Oranı 100 ile çarp.
6.  **Birikimli Yüzde ($\%C$):** Yüzdeleri toplayarak git.


örnek_2:
---

# 📊 1. Veriyi Yazalım

Tahtadaki veriler (30 gün):

```
24 32 27 23 31 33 29 25 23 28
20 26 31 22 27 33 27 23 28 29
31 35 34 22 26 28 23 35 31 27
```

Toplam gözlem sayısı:
👉 **n = 30**

---

# 📌 2. Min – Max – Range (Açıklık)

* En küçük değer = **20**
* En büyük değer = **35**

👉 Açıklık (Range):

```
R = 35 - 20 = 15
```

---

# 📌 3. Sınıf Sayısı (k)

Verilmiş:
👉 **k = 3**

---

# 📌 4. Sınıf Genişliği

Formül:

```
Sınıf genişliği = R / k = 15 / 3 = 5
```

---

# 📌 5. Sınıfları Oluştur

Başlangıç: 20

Sınıflar:

1. **20 – 25**
2. **25 – 30**
3. **30 – 35**

(Not: Son sınıfta 35 dahil edilir)

---

# 📌 6. Frekansları Say (en önemli kısım)

## 1. Sınıf (20–25)

Değerler:
20, 22, 23, 23, 23, 23, 24, 25

👉 **f₁ = 8**

---

## 2. Sınıf (25–30)

Değerler:
26, 26, 27, 27, 27, 27, 28, 28, 28, 29, 29, 25

👉 **f₂ = 12**

---

## 3. Sınıf (30–35)

Değerler:
31, 31, 31, 31, 32, 33, 33, 34, 35, 35

👉 **f₃ = 10**

---

# 📊 7. Tabloyu Oluştur (5 Frekans Türü)

| Sınıf | f (Basit) | Kümülatif f | Oransal f    | Yüzdelik (%) | Küm. Oransal |
| ----- | --------- | ----------- | ------------ | ------------ | ------------ |
| 20–25 | 8         | 8           | 8/30 = 0.27  | 26.7%        | 0.27         |
| 25–30 | 12        | 20          | 12/30 = 0.40 | 40%          | 0.67         |
| 30–35 | 10        | 30          | 10/30 = 0.33 | 33.3%        | 1.00         |

---

# 📌 8. Frekans Türlerini Anla (ÇOK ÖNEMLİ)

### 1. Basit Frekans (f)

👉 Kaç tane veri var

---

### 2. Kümülatif Frekans

👉 Üstüne ekleyerek gider

Örnek:

```
8 → 8+12=20 → 20+10=30
```

---

### 3. Oransal Frekans

👉 f / n

Örnek:

```
8/30 = 0.27
```

---

### 4. Yüzdelik Frekans

👉 Oransal × 100

```
0.27 × 100 = 27%
```

---

### 5. Kümülatif Oransal

👉 Oransal frekansların toplamı

```
0.27 → 0.27+0.40=0.67 → 1.00
```

---

# 🎯 SINAVDA ÇIKAN KRİTİK NOKTALAR

✔ Sınıf genişliği hesaplama
✔ Doğru aralık oluşturma
✔ Frekans sayarken hata yapmama
✔ Kümülatif mantığını anlama

---

# 🧠 KISA ÖZET (EZBERLE)

1. Min – Max bul
2. Range hesapla
3. k verilmiş → genişlik = R/k
4. Sınıfları oluştur
5. Say → f bul
6. Tabloyu doldur

---
