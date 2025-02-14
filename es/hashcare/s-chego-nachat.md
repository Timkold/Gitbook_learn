# 🌟 ¿Por dónde empezar?

**Agentes** es un servicio para recopilar datos sobre el estado de los dispositivos y transmitirlos al sistema de monitoreo. Ayuda a rastrear el rendimiento, la operatividad y el estado de la infraestructura para detectar problemas a tiempo.

### **🔗 Conexión:**

El agente se conecta a los dispositivos a través de protocolos (SSH, HTTP API, SNMP) y lee su estado.

### **Agente en HashCare:**

* Se instala en el servidor de la plataforma donde están ubicados los dispositivos.  
* Recoge métricas de los dispositivos en una misma red a través de direcciones IP y las envía al monitoreo.  

#### **Cómo crear un agente:**

1\. Ir al menú **Agentes**.  

2\. Hacer clic en el botón **Crear nuevo agente**.  

### **Estados de los agentes:**  

🟢 **Verde** — el agente está activo.  

🔴 **Rojo** — el agente está inactivo.  

🟡 **Amarillo** — hay agentes activos e inactivos.  

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

## **Pasos para la creación:**  

1\. Hacer clic en **Crear nuevo agente**.  

2\. En el campo **Modo**, seleccionar **Interno**.  

3\. Descargar el agente a través del enlace.  

_La guía de instalación se puede abrir desde el enlace._  

4\. Completar el campo **Nombre** (obligatorio).  

⚠️ Si el campo está vacío, el botón **Crear** no estará activo.  

<figure><img src="../.gitbook/assets/image (41).png" alt="" width="446"><figcaption></figcaption></figure>

## **🌐 Adición de subredes:**  

* El campo **Redes** no es obligatorio.  
* Formato de entrada: `XX.XX.XX.XX/XX`  
* `XX.XX.XX.XX` — dirección IP del dispositivo o subred.  
* `/XX` — máscara de subred (de 0 a 32).  

Ejemplo: `10.4.21.32/27`  

* **Dirección de red**: `10.4.21.32`  
* **Rango de hosts**: `10.4.21.33 – 10.4.21.62`  
* **Broadcast**: `10.4.21.63`  

### **➕ Para agregar subredes:**  

* Hacer clic en **Agregar** para añadir hasta 5 campos.  
* **Límite**: máximo 125,000 direcciones IP en subredes.  

## **⚙️ Instalación del agente:**  

1\. Ejecutar el comando: `<Ruta al archivo>/hashcare-agent -Dapi-key=<clave>`  

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.22.png" alt=""><figcaption></figcaption></figure>

2\. **API Key**: copiar desde el campo correspondiente.  

## 🔍 Activación del agente:  

El **agente interno** se activa tras su ejecución exitosa en el servidor.  

**Se mostrará:**  

* **🖥️ IP del agente**  
* **📜 Versión**  
* **📊 Número de dispositivos** (se actualiza cada 1–5 minutos).  

— Los dispositivos en las subredes se agregan automáticamente con sus datos completados.  

Después, puedes explorar las funcionalidades del panel de control en la sección “Hashcare”.  
