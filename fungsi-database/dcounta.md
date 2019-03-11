---
description: >-
  Pengertian, fungsi, sintaks, dan contoh penggunaan fungsi DCOUNTA pada
  Ms.Excel.
---

# DCOUNTA

## Apa itu DCOUNTA ?

     Fungsi DCOUNTA merupakan salah satu dari fungsi Database.

## Apa fungsi dari DCOUNTA ? 

     Menghitung sel-sel yang tidak kosong dalam bidang \(kolom\) rekaman dalam daftar atau database yang cocok dengan kondisi yang Anda tentukan.

## Sintaks

```text
DCOUNTA(database, bidang, kriteria)
```

{% tabs %}
{% tab title="database" %}
Rentang sel yang membentuk daftar atau database. Database adalah daftar dari data yang terkait di mana baris-baris informasi terkait adalah rekaman, dan kolom-kolom data adalah bidang. Baris pertama daftar tersebut berisi label untuk masing-masing kolom.
{% endtab %}

{% tab title="bidang" %}
Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Masukkan label kolom yang dimasukkan di antara dua tanda kutip ganda, seperti "Umur" atau "Hasil," atau angka \(tanpa tanda kutip\) yang menyatakan posisi kolom di dalam daftar: 1 untuk kolom pertama, 2 untuk kolom kedua, dan seterusnya.

{% hint style="info" %}
Opsional
{% endhint %}
{% endtab %}

{% tab title="kriteria" %}
Rentang sel berisi kondisi yang Anda tentukan. Anda dapat menggunakan rentang untuk argumen kriteria, selama meliputi setidaknya satu label kolom dan setidaknya satu sel di bawah label kolom di mana Anda menentukan kondisi untuk kolom tersebut.
{% endtab %}
{% endtabs %}

## Contoh

![](../.gitbook/assets/contohdcounta.png)

### Keterangan

{% code-tabs %}
{% code-tabs-item title="Rumus yang digunakan : " %}
```text
=DCOUNTA(A4:E10,"Profit",A1:F2)
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% tabs %}
{% tab title="database" %}
`A4:E10` menunjukan database atau data dan informasi meliputi baris dan kolom. Dalam kasus ini yaitu data Pohon, Tinggi, Umur, Hasil, dan Laba.
{% endtab %}

{% tab title="bidang" %}
`"Profit"` Mengindikasikan kolom yang digunakan dalam fungsi tersebut. Dalam kasus ini apabila menulis Profit pada bidang maka akan error karena tidak ada kolom profit. 
{% endtab %}

{% tab title="kriteria" %}
`A1:F2` merupakan sel yang berisi kriteria atau syarat yang ditentukan sendiri. Dalam kasus ini, kriterianya adalah Pohon apel yang tingginya lebih dari 10 kaki dan tidak lebih dari 16.
{% endtab %}
{% endtabs %}

