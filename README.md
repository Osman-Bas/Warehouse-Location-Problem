# 🏭 Warehouse Location Problem (WLP) - Greedy Heuristic Approach

Bu proje, **Warehouse Location Problem (WLP)** için Greedy (açgözlü) sezgisel algoritma kullanılarak geliştirilmiş bir çözüm içerir. Amaç, müşteri taleplerini karşılayacak şekilde bazı depoların açılması ve her müşterinin uygun bir depoya atanmasıyla **toplam maliyeti minimize etmektir**.

---

## 🧩 Problem Tanımı

Warehouse Location Problem (WLP), belirli sayıda müşteri ve potansiyel depo (tesis) için:

- Her deponun açılma (sabit) maliyeti vardır.
- Her müşteri, bir depoya atanmalıdır.
- Her deponun kapasitesi vardır ve bu kapasite, toplam müşteri taleplerini karşılamalıdır.
- Amaç, **toplam açma maliyetini + taşıma maliyetlerini** minimize eden bir atama yapmaktır.

---

## 📌 Kullanılan Yaklaşım

Bu çözümde **Greedy Heuristic** (Açgözlü Sezgisel) bir algoritma kullanılmıştır:

- Her müşteri, kendisini karşılayabilecek **en düşük ulaşım maliyetine sahip** depoya atanır.
- Eğer depo daha önce açılmadıysa, **sabit açma maliyeti** eklenir.
- Atamalar kapasite kısıtlarına göre yapılır.

---

## 📁 Dosya Yapısı

```bash

├── greedy_wlp.py          # Veriyi okuma ve greedy algoritmayı çalıştıran Python dosyası
├── wl_25.txt              # Örnek veri seti (25 müşteri, X depo)
├── README.md              # Proje açıklamaları
```
---

## 🧪 Veri Seti Formatı

<depo_sayısı> <müşteri_sayısı>
<kapasite> <açma_maliyeti>     # Tüm depolar için
...
<müşteri_talebi>               # Her müşteri için
<taşıma_maliyetleri>           # Her müşteri için, tüm depolara
...

## 🚀 Nasıl Çalıştırılır?

1. Gerekli dosyayı çalıştırın:
    ```bash
    python greedy_wlp.py
2.Terminal çıktısı aşağıdakine benzer olur:
```bash
 Depo Sayısı: 5
Müşteri Sayısı: 25
İlk 5 Depo Kapasitesi: [...]
İlk 5 Kurulum Maliyeti: [...]
İlk 5 Müşteri Talebi: [...]
İlk Müşterinin Ulaşım Maliyetleri (İlk 5 depo): [...]
Toplam Maliyet: 1234.56
```
## Örnek Koddan

```python
def greedy_assignment(...):
    # Her müşteri için en ucuz uygun depoyu bul
```

## 🔧 Gereksinimler

Bu proje sadece standart Python kütüphanelerini kullanır. Ekstra bağımlılık yoktur. Python 3.7+ önerilir.

## 📝 Lisans

Bu proje açık kaynaklıdır.





