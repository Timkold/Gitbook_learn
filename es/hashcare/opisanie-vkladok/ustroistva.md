# Dispositivos

Para la recopilación de datos por un agente externo, es necesario crear dispositivos con parámetros definidos. Los dispositivos se vinculan a un rack, y sin esta asociación, no es posible crearlos. Por defecto, no hay dispositivos.

### **Tabla "Dispositivos"**

• **Buscar**: ingresar caracteres para filtrar por etiqueta de activo.

• **Centro de datos, sala, rack**: filtros para seleccionar dispositivos en zonas específicas.

• **Crear nuevo dispositivo**: botón para la creación de un dispositivo.

### **Campos de la tabla**

• **ID del dispositivo**: número único del sistema.

• **Modelo**: determinado por el agente o ingresado manualmente; se muestra el firmware.

• **Tasa de hash**: rendimiento actual (TH/s):

🟢 Círculo verde: tasa de hash mayor a 0.

🔴 Círculo rojo: tasa de hash igual a 0 o no determinada.

• **Nombre del trabajador**: nombre del pool y del dispositivo (definido por el agente o manualmente).

• **Dirección IP**: detectada automáticamente o ingresada manualmente.

• **S/N**: número de serie, determinado por el agente o ingresado manualmente.

• **Ubicación**: Centro de datos / Sala / Rack (enlaces a las entidades).

• **Edición**: botón para configurar los parámetros.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

## **Creación de un dispositivo a través del formulario**

1\. Ir al menú **Dispositivos**.

2\. Hacer clic en el botón **Crear nuevo dispositivo**.

3\. En la ventana emergente, ingresar los siguientes datos:

• **Tipo de dispositivo**: modelo (menú desplegable con función de búsqueda). _Campo obligatorio._

• **Etiqueta de activo**: nombre único del dispositivo en el sistema Hashcare. _Campo obligatorio._

• **Número de serie**: _Campo obligatorio._

• **Dirección IP**: debe cumplir con el formato: ^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Campo obligatorio._

• **Dirección MAC**: debe cumplir con el formato: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Número de estante**: número del estante libre en función del rack.

* No puede ser igual a 0. _Error: "Debe ser mayor o igual a 1"._
* No puede ser mayor que el número total de estantes en el rack. _Error: "error.codes.rack\_exceed\_max\_size"._
* Debe ser un número. _Error: "Formato incorrecto"._

• **Número de lugar**: número del espacio libre en el estante.

* No puede ser igual a 0. _Error: "Debe ser mayor o igual a 1"._
* No puede ser mayor que el número total de lugares en el estante.
* Debe ser un número. _Error: "Formato incorrecto"._

• **URLs de Stratum del grupo**: hasta 3 direcciones. _Campo opcional._

• **Nombre del trabajador del grupo**: nombre del dispositivo en el pool. _Campo obligatorio._

• **Nombre del pool**: nombre del pool. _Campo obligatorio._

• **Rack**: selección de un rack existente. _Campo obligatorio._

• **Tipo de firmware**: _Campo obligatorio._

4\. Hacer clic en **Crear**.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt="" width="447"><figcaption></figcaption></figure>

## **Importación de dispositivos en lista** <a href="#importacion-de-dispositivos-en-lista" id="importacion-de-dispositivos-en-lista"></a>

1\. Ir al menú **Dispositivos**.

2\. Seleccionar la opción **Importar dispositivos (.csv)** en el menú desplegable.

3\. Seleccionar el archivo .csv en el disco duro.

4\. Si la carga es exitosa, aparecerá el mensaje "Archivo cargado con éxito".

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

**Ejemplo de tabla CSV**

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
* Может быть только цифрой. _Ошибка: “Некорректный формат.”_

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

<figure><img src="../../.gitbook/assets/image.png" alt="" width="446"><figcaption></figcaption></figure>

3\. Нажать **Обновить** для сохранения изменений.

## **Редактирование устройств через CSV файл** <a href="#redaktirovanie-ustrojstv-cherez-csv-fajl" id="redaktirovanie-ustrojstv-cherez-csv-fajl"></a>

Имеется возможность отредактировать больше одного устройства через csv файл. Для этого необходимо загрузить csv с списком устройств, которые уже есть в списке созданных.

1. Главным идентификатором будет **MAC адрес** - если MAC созданного устройства и устройства в csv файле, то остальные данные изменяются согласно информации в csv файле
2. Если MAC адреса нет в системе Hashcare - создаётся новое устройство с заданными в csv файле параметрами

## **Удаление Устройства:**

1. Нажать на кнопку (_три точки_) рядом с нужным устройством
2. Выбрать пункт меню **Удалить**
3. В открывшемся окне нажать кнопку **Подтвердить**

<figure><img src="../../.gitbook/assets/image (1).png" alt="" width="340"><figcaption></figcaption></figure>

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

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>
