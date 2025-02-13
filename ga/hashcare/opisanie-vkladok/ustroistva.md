# Gléasanna

Chun sonraí a bhailiú ag gníomhaire seachtrach, ní mór gléasanna a chruthú le paraiméadair shonraithe. Tá na gléasanna ceangailte le raca; gan nasc, ní féidir iad a chruthú. De réir réamhshocraithe, níl aon ghléasanna ann.

### **Tábla Gléasanna**

• Cuardach — cuir isteach siombailí chun scagadh de réir clibe sócmhainne.

• Ionad Sonraí, Seomra, Raca — scagairí chun gléasanna a roghnú i gceantair áirithe.

• Cruthaigh Gléas Nua — cnaipe chun gléas a chruthú.

### **Réimsí na Tábla**

• ID an Ghléis — uimhir uathúil an chórais.

• Múnla — sainmhínítear ag an ngníomhaire nó de láimh; taispeántar an firmware.

• Ráta Haisia — feidhmíocht reatha (TH/s):

🟢 Ciorcal Glas — ráta haisia níos mó ná 0.

🔴 Ciorcal Dearg — ráta haisia = 0 nó neamhshainithe.

• Ainm an Oibrí — ainm an linne agus an ghléis (sainmhínítear ag an ngníomhaire nó de láimh).

• Seoladh IP — braitear go huathoibríoch nó socraítear de láimh.

• S/N — uimhir sraitheach, braite ag an ngníomhaire nó socraithe de láimh.

• Suíomh — Ionad Sonraí / Seomra / Raca (nascanna le háiteanna).

• Nuashonrú — cnaipe chun paraiméadair a shocrú.

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

## **Cruthú Gléis tríd an bhFoirm**

1\. Téigh go **Gléasanna**.

2\. Cliceáil ar **Cruthaigh Gléas Nua**.

3\. Sa fhuinneog a osclaítear, iontráil na sonraí seo:

• **Cineál Gléis** — múnla (roghchlár anuas le cuardach). _Riachtanach._

• **Clib Sócmhainne** — ainm uathúil an ghléis sa chóras Hashcare. _Riachtanach._

• **Uimhir Sraithe** — _Riachtanach._

• **Seoladh IP** — caithfidh sé an patrún seo a leanúint:  
^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Riachtanach._

• **Seoladh MAC** — caithfidh sé an patrún seo a leanúint: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Uimhir Sceilf** — uimhir sceilf saor i raca áirithe.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1”._
* Ní féidir a bheith níos mó ná líon na sceilfeanna sa raca. _Earráid: “error.codes.rack\_exceed\_max\_size”._
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí”._

• **Uimhir Áite** — uimhir shuíomh saor ar sceilf.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1”._
* Ní féidir a bheith níos mó ná líon na suíomhanna ar an sceilf.
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí”._

• **URLanna Stratum an Linn** — suas le 3 URL. _Neamhobligáideach._

• **Ainm Oibrí an Linn** — ainm an ghléis ar an linn. _Riachtanach._

• **Ainm an Linne** — ainm an linne. _Riachtanach._

• **Raca** — rogha ó na racaí atá ann. _Riachtanach._

• **Cineál Firmware** — _Riachtanach._

4\. Cliceáil **Cruthaigh**.

<figure><img src="../../.gitbook/assets/image (27).png" alt="" width="446"><figcaption></figcaption></figure>

## **Iompórtáil Gléasanna mar Liosta** <a href="#importirovanie-ustrojstv-spiskom" id="importirovanie-ustrojstv-spiskom"></a>

1. Téigh go **Gléasanna**.
2. Roghnaigh **Iompórtáil Gléasanna (.csv)** sa roghchlár anuas.
3. Roghnaigh comhad .csv ar do thiomántán crua.
4. Má éiríonn leis an uaslódáil, taispeánfar an teachtaireacht **“D’éirigh leis an uaslódáil”**.

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1).png" alt="" width="451"><figcaption></figcaption></figure>

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
