# Racks

Un **rack** es una entidad vinculada a una sala específica y contiene un número determinado de espacios para dispositivos. Solo muestra los datos de los dispositivos dentro de él.

• Se puede crear un número ilimitado de racks en una sala.  

• Por defecto, se crea un rack vinculado a la sala creada.  

## **Tabla "Racks"**  

• **Buscar**: búsqueda por nombre.  

• **Centro de datos**: selección de racks en un centro de datos específico.  

• **Salas**: selección de racks en una sala específica.  

• **Crear nuevo rack**: botón para la creación de un rack.  

### **Campos de la tabla:**  

• **ID**: identificador en la base de datos.  

• **Nombre**: nombre del rack.  

• **Centro de datos**: nombre del centro de datos.  

• **Sala**: sala a la que está vinculado el rack.  

• **Edición**: configuración de parámetros.  

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

## **Creación de un rack**  

1\. Ir al menú **Racks**.  

2\. Hacer clic en el botón **Crear nuevo rack**.  

3\. En la ventana emergente:  

* Ingresar un nombre en el campo **Nombre**.  
* Especificar la cantidad de estantes (**Altura**) de 1 a 10.  
* Especificar la cantidad de espacios por estante (**Ancho**) de 1 a 10.  
* Seleccionar una sala del menú desplegable.  

4\. Hacer clic en **Crear**.  

<figure><img src="../../.gitbook/assets/image (31).png" alt="" width="341"><figcaption></figcaption></figure>

## **Edición de un rack**  

1\. Hacer clic en el botón ⋮ junto al rack deseado.  

2\. Seleccionar la opción **Actualizar rack**.  

3\. Realizar los cambios:  

* Nuevo nombre.  
* Cantidad de estantes (**Altura**) de 1 a 10.  
* Cantidad de espacios por estante (**Ancho**) de 1 a 10.  
* Sala a la que se vinculará el rack.  

4\. Hacer clic en **Actualizar**.  

<figure><img src="../../.gitbook/assets/image (32).png" alt="" width="340"><figcaption></figcaption></figure>

## **Eliminación de un rack**  

1\. Hacer clic en el botón ⋮ junto al rack deseado.  

2\. Seleccionar la opción **Eliminar**.  

3\. En la ventana emergente, hacer clic en **Confirmar**.  

<figure><img src="../../.gitbook/assets/image (34).png" alt="" width="341"><figcaption></figcaption></figure>

## **Acceder a la página de un rack**  

* En el menú **Racks**, hacer clic en el **Nombre** del rack deseado.  

## **Contenido de la página del rack**  

### **Detalles:**  

• **Tamaño**: ancho × altura (por ejemplo, 10×10).  

• **Número de espacios**: total (ancho × altura).  

• **Número de dispositivos**:  

* **Todos**: inactivos + en línea.  
* **En línea**: dispositivos transmitiendo datos.  

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

### **Gráficos:**  

**• Tasa de hash:**  

* **Asic Hashrate**: tasa de hash informada por el dispositivo.  
* **Nominal Hashrate**: tasa de hash declarada por el fabricante.  

**• Consumo de energía:**  

* **Asic Power**: consumo reportado por el dispositivo.  
* **Nominal Power**: consumo declarado por el fabricante.  

**• Dispositivos:**  

* **Active Asic**: dispositivos en funcionamiento.  
* **Total Asic**: cantidad total de dispositivos, incluyendo los inactivos.  

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

### **Mapa del rack**  

Muestra un esquema 2D con la cantidad de espacios definida y los dispositivos colocados.  

• En cada celda se indican:  

* La tasa de hash actual.  
* La temperatura máxima de los chips.  

• Características de la visualización:  

* Si la tasa de hash o la temperatura = 0 o supera los valores normales, el texto se muestra en rojo.  
* Para ver los problemas actuales, se puede cambiar la característica mostrada en la esquina superior derecha.  

<figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

### **Lista de dispositivos en el rack**  

Enumera los dispositivos vinculados al rack.  

• La tabla incluye:  

* **ID del dispositivo**: identificador único asignado por el sistema.  
* **Modelo**: determinado por el agente o ingresado manualmente; se muestra la versión del firmware.  
* **Tasa de hash**: rendimiento actual del dispositivo:  

  🟢 Tasa de hash > 0  
  🔴 Tasa de hash = 0 o no determinada  

* **Nombre del trabajador**: compuesto por el nombre del pool y del dispositivo, determinado por el agente o ingresado manualmente.  
* **Dirección IP**: detectada automáticamente por el agente o ingresada manualmente.  

<figure><img src="../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>
