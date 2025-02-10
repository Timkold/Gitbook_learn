# Rak

**Rak** ialah entiti yang dikaitkan dengan satu bilik dan merangkumi sejumlah ruang untuk peranti. Ia hanya memaparkan data peranti yang berada di dalamnya.

• Anda boleh mencipta bilangan rak yang tidak terhad dalam satu bilik.

• Secara lalai, satu rak akan dibuat dan dikaitkan dengan bilik yang baru dibuat.

## **Jadual “Rak”**

• **Cari** – mencari mengikut nama.

• **Pusat Data** – pemilihan rak dalam pusat data tertentu.

• **Bilik** – pemilihan rak dalam bilik.

• **Buat Rak Baru** – butang untuk mencipta rak baharu.

## **Medan Jadual:**

• **ID** – pengecam dalam pangkalan data.

• **Nama** – nama rak.

• **Pusat Data** – nama pusat data.

• **Bilik** – bilik yang dikaitkan dengan rak.

• **Edit** – konfigurasi parameter.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

## **Membuat Rak**

1\. Pergi ke menu **Rak**.

2\. Klik butang **Buat Rak Baru**.

3\. Dalam tetingkap yang dibuka:

* Masukkan nama dalam medan **Nama**.
* Tetapkan jumlah rak (**Tinggi**) dari 1 hingga 10.
* Tetapkan jumlah tempat dalam satu rak (**Lebar**) dari 1 hingga 10.
* Pilih bilik daripada senarai pilihan.

4\. Klik butang **Buat**.

<figure><img src="../../.gitbook/assets/image (28).png" alt="" width="341"><figcaption></figcaption></figure>

## **Mengemas Kini Rak**

1\. Klik butang _tiga titik_ di sebelah rak yang diperlukan.

2\. Pilih pilihan **Kemas Kini**.

3\. Buat perubahan:

* Nama baharu.
* Jumlah rak (**Tinggi**) dari 1 hingga 10.
* Jumlah tempat dalam satu rak (**Lebar**) dari 1 hingga 10.
* Bilik yang akan dikaitkan dengan rak.

4\. Klik **Kemas kini**.

<figure><img src="../../.gitbook/assets/image (29).png" alt="" width="341"><figcaption></figcaption></figure>

## **Menghapus Rak:** <a href="#menghapus-rak" id="menghapus-rak"></a>

1\. Klik butang _tiga titik_ di sebelah rak yang ingin dipadam.

2\. Pilih pilihan **Padam**.

3\. Dalam tetingkap yang muncul, klik butang **Sahkan**.

<figure><img src="../../.gitbook/assets/image (30).png" alt="" width="343"><figcaption></figcaption></figure>

## **Pergi ke Halaman Rak**

* Dalam menu **Rak**, klik pada **Nama** rak yang diperlukan.

## **Kandungan Halaman Rak**

### **Butiran:**

• **Saiz**: lebar × tinggi (contohnya, 10×10).

• **Bilangan Tempat**: jumlah keseluruhan (lebar × tinggi).

• **Bilangan Peranti**:

* **Semua** – peranti tidak aktif + dalam talian.
* **Dalam Talian** – peranti yang menghantar data.

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

### **Grafik:**

**• Kadar Hash:**

* **Asic Hashrate** – data yang dihantar oleh peranti.
* **Nominal Hashrate** – seperti yang dinyatakan oleh pengeluar.

**• Penggunaan Tenaga:**

* **Asic Power** – data yang dihantar oleh peranti.
* **Nominal Power** – seperti yang dinyatakan oleh pengeluar.

**• Peranti:**

* **Active Asic** – peranti yang sedang beroperasi.
* **Total Asic** – jumlah keseluruhan peranti, termasuk yang tidak berfungsi.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

### **Peta Rak**

Memaparkan pelan 2D dengan jumlah tempat yang ditetapkan dan peranti yang diletakkan di dalamnya.

• Setiap sel menunjukkan:

* Kadar hash sebenar.
* Suhu maksimum cip.

• Ciri paparan:

* Jika kadar hash atau suhu = 0 atau melebihi norma, teks akan berwarna merah.
* Untuk melihat masalah semasa, tukar ciri paparan di sudut kanan atas.

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

### **Senarai Peranti dalam Rak**

Menyenaraikan peranti yang dikaitkan dengan rak.

• Jadual termasuk:

* **ID Peranti** – pengecam unik yang diberikan oleh sistem.
* **Model** – ditentukan oleh ejen atau ditetapkan secara manual; firmware dipaparkan.
* **Kadar Hash** – penunjuk semasa peranti:

&#x20;     🟢 Kadar Hash > 0

&#x20;     🔴 Kadar Hash = 0 atau tidak ditentukan

* **Nama Pekerja** – terdiri daripada nama kolam dan peranti, ditentukan oleh ejen atau secara manual.
* **Alamat IP** – ditentukan secara automatik oleh ejen atau ditetapkan secara manual.

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>
