# Peranti

Untuk mengumpulkan data dengan ejen luaran, anda perlu mencipta peranti dengan parameter yang ditetapkan. Peranti dikaitkan dengan rak, dan penciptaan tanpa kaitan tidak mungkin. Secara lalai, tiada peranti yang tersedia.

### **Jadual Peranti**

• **Cari** – memasukkan aksara untuk menapis berdasarkan tag aset.

• **Pusat Data, Bilik, Rak** – penapis untuk memilih peranti dalam zon tertentu.

• **Buat Peranti Baru** – butang untuk mencipta peranti.

### **Medan Jadual**

• **ID Peranti** – nombor unik dalam sistem.

• **Model** – ditentukan oleh ejen atau ditetapkan secara manual; firmware ditunjukkan.

• **Kadar Hash** – prestasi semasa (TH/s):

🟢 Bulatan hijau – kadar hash lebih besar daripada 0.

🔴 Bulatan merah – kadar hash sama dengan 0 atau tidak ditentukan.

• **Nama Pekerja** – nama kolam dan peranti (ditentukan oleh ejen atau secara manual).

• **Alamat IP** – ditentukan secara automatik atau ditetapkan secara manual.

• **S/N** – nombor siri, ditentukan oleh ejen atau secara manual.

• **Lokasi** – Pusat Data / Bilik / Rak (pautan ke objek).

• **Edit** – butang konfigurasi parameter.

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

## **Membuat Peranti melalui Borang**

1\. Pergi ke menu **Peranti**.

2\. Klik butang **Buat Peranti Baru**.

3\. Dalam tetingkap yang dibuka, masukkan maklumat berikut:

• **Jenis Peranti** – model (menu lungsur dengan fungsi carian). _Wajib diisi._

• **Tag Aset** – nama unik peranti dalam sistem Hashcare. _Wajib diisi._

• **Nombor Siri** – _Wajib diisi._

• **Alamat IP** – mesti mematuhi corak: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Wajib diisi._

• **Alamat MAC** – mesti mematuhi corak: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Nombor Rak** – nombor rak kosong bergantung pada rak yang dipilih.

* Tidak boleh sama dengan 0. _Ralat: “Mesti lebih besar atau sama dengan 1”._
* Tidak boleh lebih besar daripada jumlah rak yang ditetapkan. _Ralat: “error.codes.rack\_exceed\_max\_size”._
* Hanya nombor dibenarkan. _Ralat: “Format tidak sah”._

• **Nombor Tempat** – nombor tempat kosong pada rak.

* Tidak boleh sama dengan 0. _Ralat: “Mesti lebih besar atau sama dengan 1”._
* Tidak boleh lebih besar daripada jumlah tempat pada rak.
* Hanya nombor dibenarkan. _Ralat: “Format tidak sah”._

• **URL Stratum Kolam** – sehingga 3 alamat. _Pilihan._

• **Nama Pekerja Kolam** – nama peranti dalam kolam. _Wajib diisi._

• **Nama Kolam** – nama kolam. _Wajib diisi._

• **Rak** – pilihan daripada rak yang sedia ada. _Wajib diisi._

• **Jenis Firmware** – _Wajib diisi._

4\. Klik **Buat**.

<figure><img src="../../.gitbook/assets/image (36).png" alt="" width="448"><figcaption></figcaption></figure>

## **Mengimport Peranti secara Senarai** <a href="#mengimport-peranti" id="mengimport-peranti"></a>

1\. Pergi ke menu **Peranti**.

2\. Pilih dalam menu lungsur **Import Peranti (.csv)**.

3\. Pilih fail **.csv** daripada cakera keras.

4\. Jika muat naik berjaya, mesej **"Fail berjaya dimuat naik"** akan dipaparkan.

<figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

## **Contoh Jadual CSV**

<figure><img src="../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

## **Kemas Kini Peranti**

1\. Klik butang **(tiga titik)** di sebelah peranti yang ingin dikemas kini.

2\. Pilih pilihan **Kemas Kini**.

_**Parameter yang boleh dikemas kini:**_

• **Jenis Peranti** – model. Medan ini berfungsi sebagai menu lungsur dengan fungsi carian. _Wajib diisi._

• **Tag Aset** – nama unik peranti dalam sistem Hashcare. _Wajib diisi._

• **Nombor Siri** – _Wajib diisi._

• **Alamat IP** – mesti mematuhi corak: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Wajib diisi._

• **Alamat MAC** – mesti mematuhi corak: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$. _Wajib diisi._

• **Nombor Rak** – nombor rak kosong bergantung pada rak yang dipilih.

* Tidak boleh sama dengan 0. _Ralat: “Mesti lebih besar atau sama dengan 1.”_
* Tidak boleh lebih besar daripada jumlah rak yang ditetapkan. _Ralat: “error.codes.rack\_exceed\_max\_size.”_
* Hanya nombor dibenarkan. _Ralat: “Format tidak sah.”_

• **Nombor Tempat** – nombor tempat kosong pada rak.

* Tidak boleh sama dengan 0. _Ralat: “Mesti lebih besar atau sama dengan 1.”_
* Tidak boleh lebih besar daripada jumlah tempat yang ditetapkan pada rak. _Ralat: “Format tidak sah.”_
* Hanya nombor dibenarkan. _Wajib diisi._

• **URL Stratum Kolam** – alamat Stratum. Sehingga 3 alamat boleh ditambah. _Pilihan._

• **Nama Pekerja Kolam** – nama peranti dalam kolam. _Wajib diisi._

• **Nama Kolam** – nama kolam. _Wajib diisi._

• **Rak** – pemilihan daripada rak sedia ada. _Wajib diisi._

• **Jenis Firmware** – _Wajib diisi._

• **Ubah bilangan rak** (**Tinggi**) – mesti lebih besar atau sama dengan 1 dan kurang atau sama dengan 10.

• **Ubah bilangan tempat dalam rak** (**Lebar**) – mesti lebih besar atau sama dengan 1 dan kurang atau sama dengan 10.

• **Ubah bilik** yang dikaitkan dengan rak.

<figure><img src="../../.gitbook/assets/image.png" alt="" width="446"><figcaption></figcaption></figure>

3\. Klik **Kemas Kini** untuk menyimpan perubahan.

## **Kemas Kini Peranti melalui Fail CSV** <a href="#kemas-kini-peranti-melalui-fail-csv" id="kemas-kini-peranti-melalui-fail-csv"></a>

Anda boleh mengemas kini lebih daripada satu peranti menggunakan fail CSV. Untuk melakukannya, muat naik fail CSV dengan senarai peranti yang sudah wujud dalam sistem.

1. **Alamat MAC** akan menjadi pengecam utama – jika MAC dalam fail CSV sepadan dengan yang sudah ada dalam sistem Hashcare, data lain akan dikemas kini berdasarkan fail CSV.
2. Jika alamat MAC tidak wujud dalam sistem Hashcare, peranti baharu akan dibuat berdasarkan data dalam fail CSV.

## **Padam Peranti:**

1. Klik butang **(tiga titik)** di sebelah peranti yang ingin dipadam.
2. Pilih pilihan **Padam**.
3. Dalam tetingkap yang muncul, klik butang **Sahkan**.

<figure><img src="../../.gitbook/assets/image (1).png" alt="" width="342"><figcaption></figcaption></figure>

## **Butiran Peranti:**

• **Model**

Ditentukan secara automatik oleh ejen dalaman atau ditetapkan secara manual dalam tetapan peranti. Termasuk kadar hash kilang.

• **Alamat IP**

Ditentukan secara automatik oleh ejen dalaman semasa pemantauan rangkaian atau ditetapkan secara manual dalam tetapan peranti.

• **Firmware**

Ditentukan secara automatik oleh ejen dalaman semasa pemantauan peranti atau ditetapkan secara manual dalam tetapan peranti.

• **Nombor Siri (S/N)**

Ditentukan secara automatik oleh ejen dalaman semasa pemantauan peranti atau ditetapkan secara manual dalam tetapan peranti.

### **Kuasa**

• **Kuasa Nominal**

Nilai statik yang ditetapkan untuk setiap model peranti.

* **W/TH** – nilai relatif yang dikira sebagai nisbah penggunaan kuasa nominal kepada kadar hash nominal model.

• **Kadar Hash Nominal**

Nilai kadar hash kilang yang diperoleh oleh ejen dalaman daripada ASIC.

### **Maklumat Tambahan**

• **Nama Pekerja**

Terdiri daripada nama kolam dan nama peranti dalam kolam. Ditentukan secara automatik oleh ejen dalaman atau ditetapkan secara manual dalam tetapan peranti.

• **Alamat MAC**

Ditentukan secara automatik oleh ejen dalaman semasa pemantauan peranti atau ditetapkan secara manual dalam tetapan peranti.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### **Показатели:**

**• Оценочный доход (PPS | FPPS):**

* PPS (Pay Per Share): фиксированная оплата за доли.
* FPPS (Full Pay Per Share): включает доход от комиссий, выше PPS.

**• Доход из пула:**

Реальный доход от пула за выбранный период.

_Настройка пула: «Настройка пулов» → Создать пул._

**• Затраты на электричество:**

Основаны на мощности устройства и тарифе:\\

(Потребляемая мощность (W) × 24) ÷ 1000 × Тариф\\

**• Прибыль:**

{FPPS доход} - {Электричество}

### **График хэшрейта**

• **Asic Hashrate** — текущий хэшрейт, переданный устройством.

• **Nominal Hashrate** — заявленный производителем хэшрейт.

### **График хэшрейта плат**

Показывает производительность отдельных плат ASIC-майнера.

• Каждая плата обозначается, например, как SM 0, SM 1, SM 2.

• Помогает выявить неисправности, снижающие общий хэшрейт.

### **Температура устройства**

• Температура плат (boards) и чипов (chip, PCB): отображает нагрев отдельных компонентов устройства.

• Температура воздуха (in/out):

* **In** — температура входящего холодного воздуха.
* **Out** — температура выходящего нагретого воздуха.

### **График скорости вентиляторов**

Показывает обороты охлаждающих вентиляторов в минуту (RPM).

* **In** — вентиляторы на входе воздушного потока.
* **Out** — вентиляторы на выходе.

### **График потребления электроэнергии**

* **Asic Power** — текущее потребление, переданное устройством.
* **Nominal Power** — заявленное производителем потребление.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
