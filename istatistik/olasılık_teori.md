
---

# Olasılık Sınav Hazırlık Notları

## 1. Temel Kavramlar

* **Deney:** Sonucu kesin olarak kestirilemeyen sürece denir.
* **Örnek Uzay ($S$):** Bir deneyde çıkabilecek tüm sonuçların kümesidir.
* **Olay ($A$):** Örnek uzayın herhangi bir alt kümesidir.
* **Olasılık Fonksiyonu:** Bir $A$ olayının gerçekleşme olasılığı $P(A)$ ile gösterilir ve şu şekilde hesaplanır:

$$P(A) = \frac{s(A)}{s(S)} = \frac{\text{İstenen Durum Sayısı}}{\text{Tüm Durumların Sayısı}}$$



> **Not:** Bir olayın olasılığı her zaman $0 \leq P(A) \leq 1$ aralığındadır. $P(A)=0$ ise imkansız olay, $P(A)=1$ ise kesin olaydır.

---

## 2. Ayrık Olaylar (Mutually Exclusive Events)

Aynı anda gerçekleşmesi mümkün olmayan olaylardır. İki olay ayrık ise kesişimleri boş kümedir ($A \cap B = \emptyset$).

**Birleşim Formülü:**
İki olay ayrık ise, bu olaylardan birinin veya diğerinin gerçekleşme olasılığı:


$$P(A \cup B) = P(A) + P(B)$$

**Örnek:** Bir zar atıldığında üst yüze gelen sayının 1 veya 6 gelme olasılığı:

* $P(1) = 1/6$
* $P(6) = 1/6$
* $P(1 \cup 6) = 1/6 + 1/6 = 2/6 = 1/3$

---

## 3. Ayrık Olmayan Olaylar

Eğer iki olay aynı anda gerçekleşebiliyorsa (kesişimleri varsa), birleşim olasılığı hesaplanırken ortak durumlar bir kez çıkarılır.

**Genel Birleşim Formülü:**


$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

**Örnek:** Bir zar atıldığında üst yüze gelen sayının çift veya asal olma olasılığı:

* Çift sayılar: $\{2, 4, 6\} \rightarrow P(A) = 3/6$
* Asal sayılar: $\{2, 3, 5\} \rightarrow P(B) = 3/6$
* Hem çift hem asal: $\{2\} \rightarrow P(A \cap B) = 1/6$
* $P(A \cup B) = 3/6 + 3/6 - 1/6 = 5/6$

---

## 4. Bağımsız Olaylar (Independent Events)

Bir olayın gerçekleşmesi, diğer olayın gerçekleşme olasılığını etkilemiyorsa bu olaylar bağımsızdır.

**Kesişim Formülü:**


$$P(A \cap B) = P(A) \cdot P(B)$$

**Örnek:** Bir madeni para ve bir zar aynı anda atılıyor. Paranın Tura ($T$) ve zarın 5 gelme olasılığı:

* $P(T) = 1/2$
* $P(5) = 1/6$
* $P(T \cap 5) = (1/2) \cdot (1/6) = 1/12$

---

## 5. Koşullu Olasılık (Conditional Probability)

Bir $A$ olayının gerçekleştiği bilindiğine göre, $B$ olayının gerçekleşme olasılığıdır. Bu durum örnek uzayı $S$'den $A$'ya daraltır.

**Koşullu Olasılık Formülü:**


$$P(B|A) = \frac{P(A \cap B)}{P(A)}$$

**Örnek:** Bir çift zar atılıyor. Toplamın 8 olduğu bilindiğine göre, zarlardan en az birinin 2 olma olasılığı:

* Toplamı 8 olanlar ($A$): $\{(2,6), (6,2), (3,5), (5,3), (4,4)\} \rightarrow s(A) = 5$
* Bu grupta en az bir tane 2 olanlar ($A \cap B$): $\{(2,6), (6,2)\} \rightarrow s(A \cap B) = 2$
* $P(B|A) = 2/5$

---




