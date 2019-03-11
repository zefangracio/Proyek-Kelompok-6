---
description: 'Pengertian, fungsi, sintaks, dan contoh penggunaan fungsi DGET pada Ms.Excel.'
---

# DGET

## Apa itu DGET ? <a id="apa-itu-dcount"></a>

 Fungsi DGET merupakan salah satu dari fungsi Database.

## Apa fungsi dari DGET ?  <a id="apa-fungsi-dari-dcount"></a>

 Menghitung sel-sel yang berisi angka dalam bidang \(kolom\) rekaman dalam daftar atau database yang cocok dengan syarat yang ditentukan.

## Sintaks <a id="sintaks"></a>

```text
DGET(database, bidang, kriteria)
```

{% tabs %}
{% tab title="database" %}
Rentang sel yang membentuk daftar atau database. Database adalah daftar dari data yang terkait di mana baris-baris informasi terkait adalah rekaman, dan kolom-kolom data adalah bidang. Baris pertama daftar tersebut berisi label untuk masing-masing kolom.
{% endtab %}

{% tab title="bidang" %}
Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Masukkan label kolom yang dimasukkan di antara dua tanda kutip ganda, seperti "Umur" atau "Hasil," atau angka \(tanpa tanda kutip\) yang menyatakan posisi kolom di dalam daftar: 1 untuk kolom pertama, 2 untuk kolom kedua, dan seterusnya.
{% endtab %}

{% tab title="kriteria" %}
Rentang sel berisi kondisi yang Anda tentukan. Anda dapat menggunakan rentang untuk argumen kriteria, selama meliputi setidaknya satu label kolom dan setidaknya satu sel di bawah label kolom di mana Anda menentukan kondisi untuk kolom tersebut.
{% endtab %}
{% endtabs %}

## Contoh <a id="contoh"></a>

![](../.gitbook/assets/dget.JPG)

### Keterangan <a id="keterangan"></a>

* Jika tidak ada rekaman yang cocok dengan kriteria, DGET akan mengembalikan nilai kesalahan \#VALUE!.
* Jika lebih dari satu rekaman yang cocok dengan kriteria, DGET akan mengembalikan nilai kesalahan \#NUM!.

{% code-tabs %}
{% code-tabs-item title="Rumus yang digunakan : " %}
```text
=DGET(A5:E10,"Hasil",A1:F3)
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% tabs %}
{% tab title="database" %}
`A5:E10` menunjukan database atau data dan informasi meliputi baris dan kolom. Dalam kasus ini yaitu data Pohon, Tinggi, Umur, Hasil, dan Laba.
{% endtab %}

{% tab title="bidang" %}
`"Hasil"` Mengindikasikan kolom yang digunakan dalam fungsi tersebut. 
{% endtab %}

{% tab title="kriteria" %}
`A1:F2` merupakan sel yang berisi kriteria atau syarat yang ditentukan sendiri. Dalam kasus ini, kriterianya adalah Pohon apel yang tingginya lebih dari 10 kaki dan tidak lebih dari 16.
{% endtab %}
{% endtabs %}



