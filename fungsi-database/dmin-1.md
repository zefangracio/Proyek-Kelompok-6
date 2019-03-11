---
description: 'Pengertian, fungsi, sintaks, dan contoh penggunaan fungsi DMIN pada Ms.Excel'
---

# DMIN

## Apa itu DMIN ?

Fungsi DMIN merupakan salah satu dari fungsi Database.

## Apa fungsi dari DMIN ? 

Mengembalikan angka terkecil dalam bidang \(kolom\) rekaman dalam daftar atau database yang cocok dengan dengan kondisi yang Anda tentukan.

## Sintaks

```text
DMIN(database, field, criteria)
```

{% tabs %}
{% tab title="database" %}
Rentang sel yang membentuk daftar atau database. Database adalah daftar dari data yang terkait di mana baris-baris informasi terkait adalah rekaman, dan kolom-kolom data adalah bidang. Baris pertama daftar tersebut berisi label untuk masing-masing kolom.
{% endtab %}

{% tab title="field" %}
Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Masukkan label kolom yang dimasukkan di antara dua tanda kutip ganda, seperti "Umur" atau "Hasil," atau angka \(tanpa tanda kutip\) yang menyatakan posisi kolom di dalam daftar: 1 untuk kolom pertama, 2 untuk kolom kedua, dan seterusnya.
{% endtab %}

{% tab title="criteria" %}
Rentang sel berisi kondisi yang Anda tentukan. Anda dapat menggunakan rentang untuk argumen kriteria, selama meliputi setidaknya satu label kolom dan setidaknya satu sel di bawah label kolom di mana Anda menentukan kondisi untuk kolom tersebut.
{% endtab %}
{% endtabs %}

## Contoh

![](../.gitbook/assets/dmin.JPG)

### Keterangan

{% code-tabs %}
{% code-tabs-item title="Rumus yang digunakan : " %}
```text
=DMIN(A5:E10, "Profit", A1:F3)
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% tabs %}
{% tab title="database" %}
`A5:E10` menunjukan database atau data dan informasi meliputi baris dan kolom. Dalam kasus ini yaitu data Pohon, Tinggi, Umur, Hasil, dan Laba.
{% endtab %}

{% tab title="bidang" %}
`"Profit"` Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Dalam kasus ini adalah Profit.
{% endtab %}

{% tab title="kriteria" %}
`A1:F3` Profit minimum dari salah satu pohon apel dengan tinggi antara 10 dan 16 kaki, atau pohon pir mana pun. Pohon apel dalam baris 9 memenuhi ketentuan ini.
{% endtab %}
{% endtabs %}

