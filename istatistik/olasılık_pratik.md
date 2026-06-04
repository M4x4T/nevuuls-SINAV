
---



## 1. Temel Deneyler ve Örnek Uzay

* **Para Atma Deneyi:** $S = \{Yazı, Tura\}$, $P(A) = \frac{1}{2}$
* **Zar Atma Deneyi:** $S = \{1, 2, 3, 4, 5, 6\}$, $P(A) = \frac{1}{6}$

### Örnek 1: 3 Para Atma Deneyi

3 para atma denemesinde olaylar şöyledir:

* **A:** En az 1 Tura gelmesi
* **B:** En fazla 1 Yazı gelmesi
* **C:** Üst yüze gelen değerlerin aynı olması

**Çözüm:**
Tüm durumlar: $n(S) = 2^3 = 8$
$S = \{TTT, TTY, TYT, YTT, TYY, YTY, YYT, YYY\}$

* $s(A) = \{TTT, TTY, TYT, YTT, YYT, YTY, TYY\} \rightarrow n(A) = 7$

$$P(A) = \frac{7}{8}$$


* $s(B) = \{TTT, TYT, TTY, YTT\} \rightarrow n(B) = 4$

$$P(B) = \frac{4}{8}$$


* $s(C) = \{TTT, YYY\} \rightarrow n(C) = 2$

$$P(C) = \frac{2}{8}$$



**Birleşim ve Kesişimler:**

* $P(A \cup B) = \frac{7}{8}$
* $P(A \cap B) = \{TYT, YTT, TTT, TTY\} \rightarrow \frac{4}{8}$
* $P(A \cap C) = \{TTT\} \rightarrow \frac{1}{8}$
* $P(B \cup C) = \{TTY, YTT, TYT, TTT, YYY\} \rightarrow \frac{5}{8}$

---

### Örnek 2: İki Zarın Atılması

Bir tavla zarı art arda iki kez atılıyor ($n(S) = 6^2 = 36$).

* **A:** Üst yüze gelen sayılar toplamı 9 olması
* **B:** Üst yüze gelen sayılar farkının 1 olması
* **C:** Üst yüze gelen sayıların aynı olması

**Olay Elemanları:**

* **A için:** $(3,6), (4,5), (5,4), (6,3) \rightarrow P(A) = \frac{4}{36}$
* **B için:** $(6,5), (5,4), (4,3), (3,2), (2,1), (5,6), (4,5), (3,4), (2,3), (1,2) \rightarrow P(B) = \frac{10}{36}$
* **C için:** $(1,1), (2,2), (3,3), (4,4), (5,5), (6,6) \rightarrow P(C) = \frac{6}{36}$

**Birleşim ve Kesişim:**

* $A \cup C = \{(3,6), (4,5), (5,4), (6,3), (1,1), (2,2), (3,3), (4,4), (5,5), (6,6)\} \rightarrow \frac{10}{36}$
* $A \cup B = \{(3,6), (4,5), (5,4), (6,3), (6,5), (4,3), (2,1), (3,4)\} \rightarrow \frac{12}{36}$
* $A \cap B = \{(5,4), (4,5)\} \rightarrow \frac{2}{36}$ (Not: El yazısında bir hata olabilir, $5-4=1$ ve $4+5=9$ olduğundan 2 tane ortak eleman vardır).

---

## 2. Tablo Soruları ve Koşullu Olasılık

### Örnek 3: Şehir ve Sigorta

700 çalışanın bulunduğu bir iş yerinde durum tablosu:

| Durum | Kadın (K) | Erkek (E) | Toplam |
| --- | --- | --- | --- |
| Evli (X) | 120 | 100 | 220 |
| Bekar (B) | 160 | 320 | 480 |
| **Toplam** | 280 | 420 | 700 |

* **A) Erkek çalışan olma olasılığı:**

$$P(E) = \frac{420}{700}$$


* **B) Erkek veya evli olma olasılığı:**

$$P(E \cup X) = P(E) + P(X) - P(E \cap X) = \frac{420}{700} + \frac{220}{700} - \frac{100}{700} = \frac{540}{700}$$


* **C) Evli ve kadın olma olasılığı:**

$$P(X \cap K) = \frac{120}{700}$$


* **D) Kadın olduğu bilindiğine göre bekar olma olasılığı:**

$$P(B|K) = \frac{P(B \cap K)}{P(K)} = \frac{160/700}{280/700} = \frac{160}{280}$$



---

### Örnek 4: Mahalle Verileri

| Durum | Ev Sahibi (E) | Kiracı (K) | Toplam |
| --- | --- | --- | --- |
| Memur (M) | 105 | 110 | 215 |
| Memur Değil (D) | 15 | 30 | 45 |
| **Toplam** | 120 | 140 | 260 |

* **A) Memur bir kiracı olma olasılığı:** $P(M \cap K) = \frac{110}{260}$
* **B) Ev sahibi veya memur olmama olasılığı:** $P(E \cup D) = P(E) + P(D) - P(E \cap D) = \frac{120}{260} + \frac{45}{260} - \frac{15}{260} = \frac{150}{260}$
* **C) Kiracı olduğu bilindiğine göre memur olma olasılığı:** $P(M|K) = \frac{110}{140}$
* **D) Memur olmadığı bilindiğine göre kiracı olma olasılığı:** $P(K|D) = \frac{30}{45}$

---

## 3. Bağımsız Olaylar ve Risk Analizi

### Örnek 5: Sigorta Ödemesi (Risk Tahmini)

Üç müşterinin (İstanbul, Ankara, İzmir) 2023 sonuna kadar yaşama olasılıkları: $P(İ) = 0.80$, $P(A) = 0.60$, $P(Z) = 0.30$.
(Not: Sigorta ödemesi, kişinin vefatı durumunda yapılır; yani yaşama olasılığının tersi ($1-P$) ödeme olasılığıdır.)

* **A) 3 müşterisine de sigorta ödemesi yapılması:**

$$P(İ' \cap A' \cap Z') = 0.20 \cdot 0.40 \cdot 0.70 = 0.056 = \%5.6$$


* **B) 3 müşterisine de ödeme yapılmaması (Hepsinin yaşaması):**

$$P(İ \cap A \cap Z) = 0.80 \cdot 0.60 \cdot 0.30 = 0.144 = \%14.4$$


* **C) Müşterilerden sadece 2'sine ödeme yapılması:**

$$(0.20 \cdot 0.40 \cdot 0.30) + (0.20 \cdot 0.60 \cdot 0.70) + (0.80 \cdot 0.40 \cdot 0.70)$$


$$= 0.024 + 0.084 + 0.224 = 0.332 = \%33.2$$



---

### Örnek 6: Hastane Sıralaması

Kapadokya ($K$), Acıbadem ($A$) ve Venesa ($V$) hastanelerinin listeye girme olasılıkları: $P(K)=0.60$, $P(A)=0.90$, $P(V)=0.70$.

* **A) 3 hastanenin de listeye girmesi:**

$$0.60 \cdot 0.90 \cdot 0.70 = 0.378 = \%37.8$$


* **B) Sadece 2 hastanenin girmesi:**

$$(K, A, V') + (K, A', V) + (K', A, V)$$


$$(0.60 \cdot 0.90 \cdot 0.30) + (0.60 \cdot 0.10 \cdot 0.70) + (0.40 \cdot 0.90 \cdot 0.70)$$


$$= 0.162 + 0.042 + 0.252 = 0.456 = \%45.6$$


* **C) En fazla 1 hastanenin girmesi (1 veya 0):**

$$(0.60 \cdot 0.10 \cdot 0.30) + (0.40 \cdot 0.90 \cdot 0.30) + (0.40 \cdot 0.10 \cdot 0.70) + (0.40 \cdot 0.10 \cdot 0.30)$$


$$= 0.018 + 0.108 + 0.028 + 0.012 = 0.166 = \%16.6$$