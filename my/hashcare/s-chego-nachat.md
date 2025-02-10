# 🌟 Bagaimana untuk memulakan?

**Ejen** ialah perkhidmatan untuk mengumpulkan data tentang keadaan peranti dan menghantarnya ke dalam sistem pemantauan. Ia membantu menjejaki prestasi, kebolehoperasian, dan keadaan infrastruktur untuk mengesan masalah dengan segera.

### **🔗 Sambungan:**

Ejen bersambung ke peranti melalui protokol (SSH, HTTP API, SNMP) dan membaca statusnya.

### **Ejen dalam HashCare:**

* Dipasang pada pelayan lokasi di mana peranti ditempatkan.
* Membaca metrik daripada peranti dalam satu rangkaian melalui alamat IP dan menghantarnya ke pemantauan.

#### **Cara mencipta ejen:**

1\. Pergi ke menu **Ejen**.

2\. Klik butang **Buat Ejen Baru**.

### **Status ejen:**

🟢 **Hijau** – ejen aktif.

🔴 **Merah** – ejen tidak aktif.

🟡 **Kuning** – terdapat ejen aktif dan tidak aktif.

<figure><img src="../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

## **Langkah-langkah untuk mencipta:**

1\. Klik butang **Buat Ejen Baru**.

2\. Dalam medan **Mod**, pilih **Dalaman**.

3\. Muat turun ejen melalui pautan.

_Anda boleh membuka arahan pemasangan melalui pautan._

4\. Isikan medan **Nama** (wajib).

⚠️ Jika medan kosong, butang **Buat** tidak akan diaktifkan.

<figure><img src="../.gitbook/assets/image (40).png" alt="" width="448"><figcaption></figcaption></figure>

## **🌐 Menambah Subnet:**

* Medan **Rangkaian** tidak wajib diisi.
* Format input: `XX.XX.XX.XX/XX`
* `XX.XX.XX.XX` – alamat IP peranti atau subnet.
* `/XX` – mask subnet (dari 0 hingga 32).

Contoh: `10.4.21.32/27`

* **Alamat Rangkaian**: `10.4.21.32`
* **Julat Hos**: `10.4.21.33 – 10.4.21.62`
* **Broadcast**: `10.4.21.63`

### **➕ Untuk menambah subnet:**

* Klik **Tambah** untuk menambah sehingga 5 medan.
* **Had**: maksimum 125,000 alamat IP dalam subnet.

## **⚙️ Pemasangan Ejen:**

1\. Jalankan perintah: `<Laluan ke fail>/hashcare-agent -Dapi-key=<kunci>`

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.22.png" alt=""><figcaption></figcaption></figure>

2\. **Kunci API**: salin daripada medan yang sesuai.

## 🔍 Pengaktifan Ejen:

**Ejen Dalaman** akan diaktifkan selepas berjaya dijalankan pada pelayan.

**Maklumat yang dipaparkan:**

* **🖥️ IP ejen**
* **📜 Versi**
* **📊 Bilangan peranti** (dikemas kini dalam masa 1–5 minit).

— Peranti dari subnet akan ditambah secara automatik dengan data mereka diisi.

Selepas itu, anda boleh meneroka fungsi dalam akaun peribadi anda di bahagian **"HashCare"**.
