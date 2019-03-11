---
description: 'Pengertian, fungsi, sintaks, dan contoh penggunaan fungsi DVAR pada Ms.Excel'
---

# DVAR

## Apa itu DVAR ?

Fungsi DVAR merupakan salah satu dari fungsi Database.

## Apa fungsi dari DVAR ? 

Memperkirakan varians populasi berdasarkan sampel dengan menggunakan angka dalam bidang \(kolom\) rekaman dalam daftar atau database yang cocok dengan kondisi yang Anda tentukan.

## Sintaks

```text
DVAR(database, field, criteria)
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

![](../.gitbook/assets/contohdvar.png)

### Keterangan

{% code-tabs %}
{% code-tabs-item title="Rumus yang digunakan :" %}
```text
=DVAR(A4:E10;"Hasil";A1:A3)
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% tabs %}
{% tab title="database" %}
`A4:E10` menunjukan database atau data dan informasi meliputi baris dan kolom. Dalam kasus ini yaitu data Pohon, Tinggi, Umur, Hasil, dan Laba.
{% endtab %}

{% tab title="field" %}
`"Hasil"` Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Dalam kasus ini adalah Hasil.
{% endtab %}

{% tab title="criteria" %}
`A1:A3` merupakan sel yang berisi kriteria atau syarat yang ditentukan sendiri. Dalam kasus ini, Perkiraan varians dalam hasil pohon apel dan pir jika data dalam database hanyalah sampel dari total populasi kebun buah-buahan.
{% endtab %}
{% endtabs %}

