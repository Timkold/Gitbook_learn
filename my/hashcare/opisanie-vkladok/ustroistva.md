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

**Пример CSV таблицы**

<figure><img src="../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

## **Редактирование устройства**

1\. Нажать на кнопку (три точки) рядом с нужным устройством.

2\. Выбрать пункт **Изменить**.

_**Доступные для изменения параметры:**_

• **Тип устройства** — модель. Поле работает как выпадающее меню с функцией поиска по символам. _Обязательно для заполнения._

• **Тэг актива** — уникальное имя устройства в системе Hashcare. _Обязательно для заполнения._

• **Серийный номер** — _Обязательно для заполнения._

• **IP-адрес** — должен соответствовать шаблону: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Обязательно для заполнения._

• **MAC-адрес** — должен соответствовать шаблону: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$. _Обязательно для заполнения._

• **Номер полки** — номер свободной полки в зависимости от выбранного стеллажа.

* Не может быть равным 0. _Ошибка: “Должно быть больше или равно 1.”_
* Не может быть больше, чем заданное количество полок в стеллаже. _Ошибка: “error.codes.rack\_exceed\_max\_size.”_
* Может быть только цифрой. _Ошибка: “Некорректный формат.”_&#x20;

• **Номер места** — номер свободного места на полке.

* Не может быть равным 0. _Ошибка: “Должно быть больше или равно 1.”_
* Не может быть больше, чем заданное количество мест на указанной полке. _Ошибка: “Некорректный формат.”_
* Может быть только цифрой. _Обязательно для заполнения._

• **Пул Stratum URLs** — Стратум адреса. Может быть добавлено от 1 до 3 адресов. _Необязательно для заполнения._

• **Имя воркера пула** — наименование устройства на пуле. _Обязательно для заполнения._

• **Имя пула** — название пула. _Обязательно для заполнения._

• **Стеллаж** — выбор из существующих стеллажей. _Обязательно для заполнения._

• **Тип прошивки** — _Обязательно для заполнения._

• **Изменить кол-во полок** (Высота) — должно быть больше или равно 1 и меньше либо равно 10.

• **Изменить кол-во мест на полках** (Ширина) — должно быть больше или равно 1 и меньше либо равно 10.

• **Изменить помещение**, к которому будет привязан стеллаж.

<figure><img src="../../.gitbook/assets/image (4).png" alt="" width="451"><figcaption></figcaption></figure>

3\. Нажать **Обновить** для сохранения изменений.

## **Редактирование устройств через CSV файл** <a href="#redaktirovanie-ustrojstv-cherez-csv-fajl" id="redaktirovanie-ustrojstv-cherez-csv-fajl"></a>

Имеется возможность отредактировать больше одного устройства через csv файл. Для этого необходимо загрузить csv с списком устройств, которые уже есть в списке созданных.

1. Главным идентификатором будет **MAC адрес** - если MAC созданного устройства и устройства в csv файле, то остальные данные изменяются согласно информации в csv файле
2. Если MAC адреса нет в системе Hashcare - создаётся новое устройство с заданными в csv файле параметрами

## **Удаление Устройства:**

1. Нажать на кнопку (_три точки_) рядом с нужным устройством
2. Выбрать пункт меню **Удалить**
3. В открывшемся окне нажать кнопку **Подтвердить**

<figure><img src="../../.gitbook/assets/image (5).png" alt="" width="344"><figcaption></figcaption></figure>

## **Детали устройства:**

• **Модель**

Автоматически определяется внутренним агентом или задаётся вручную в настройках устройства. Включает заводской хэшрейт.

• **IP-адрес**

Автоматически определяется внутренним агентом при опросе сети или задаётся вручную в настройках устройства.

• **Прошивка**

Автоматически определяется внутренним агентом при опросе устройства или задаётся вручную в настройках устройства.

• **Серийный номер (S/N)**

Автоматически определяется внутренним агентом при опросе устройства или задаётся вручную в настройках устройства.

### **Мощность**

• **Номинальная мощность**

Статичное значение, установленное для каждой модели устройства.

* W/TH - относительная величина, рассчитываемая как отношение номинального потребления к номинальному хэшрейту модели.

• **Номинальный хэшрейт**

Значение заводского хэшрейта, полученное внутренним агентом из ASIC.

### **Дополнительная информация**

• **Имя воркера**

Состоит из имени пула и имени устройства на пуле. Определяется автоматически внутренним агентом или задаётся вручную в настройках устройства.

• **MAC-адрес**

Автоматически определяется внутренним агентом при опросе устройства или задаётся вручную в настройках устройства.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

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
