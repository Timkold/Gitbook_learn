# 🌟 Por onde começar?

**Agentes** são um serviço para coletar dados sobre o estado dos dispositivos e transmiti-los ao sistema de monitoramento. Ele ajuda a rastrear o desempenho, a operabilidade e o estado da infraestrutura para detectar problemas a tempo.

### **🔗 Conexão:**

O agente se conecta aos dispositivos através de protocolos (SSH, HTTP API, SNMP) e lê seu estado.

### **Agente no HashCare:**

* É instalado no servidor do local onde os dispositivos estão hospedados.
* Lê métricas dos dispositivos na mesma rede por meio de endereços IP e as transmite para o monitoramento.

#### **Como criar um agente:**

1. Acesse o menu **Agentes**.
2. Clique no botão **Crie um novo agente**.

### **Status dos agentes:**

🟢 **Verde** — agente ativo.

🔴 **Vermelho** — agente inativo.

🟡 **Amarelo** — existem agentes ativos e inativos.

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

## **Passos para criação:**

1. Clique no botão **Crie um novo agente**.
2. No campo **Modo**, selecione **Interno**.
3. Baixe o agente pelo link.

_A instrução de instalação pode ser acessada pelo link._

4. Preencha o campo **Nome** (obrigatório).

⚠️ Se o campo estiver vazio, o botão **Criar** ficará inativo.

<figure><img src="../.gitbook/assets/image (31).png" alt="" width="447"><figcaption></figcaption></figure>

## **🌐 Adição de sub-redes:**

* O campo **Redes** não é obrigatório.
* Formato de entrada: `XX.XX.XX.XX/XX`
* `XX.XX.XX.XX` — Endereço IP do dispositivo ou da sub-rede.
* `/XX` — Máscara da sub-rede (de 0 a 32).

Exemplo: `10.4.21.32/27`

* **Endereço de rede**: `10.4.21.32`
* **Intervalo de hosts**: `10.4.21.33 – 10.4.21.62`
* **Broadcast**: `10.4.21.63`

### **➕ Para adicionar sub-redes:**

* Clique em **Adicionar** para adicionar até 5 campos.
* **Limite**: máximo de 125.000 endereços IP em sub-redes.

## **⚙️ Instalação do agente:**

1. Execute o comando: \<File path>/hashcare-agent -Dapi-key=\<key>

<figure><img src="../.gitbook/assets/Снимок экрана 2025-01-13 в 15.17.22.png" alt=""><figcaption></figcaption></figure>

2. **API Key**: copie do campo correspondente.

## 🔍 Ativação do agente:

O **Agente Interno** é ativado após a execução bem-sucedida no servidor.

**É exibido:**

* **🖥️** Endereço IP
* **📜 Versão**
* **📊** Número de dispositivos sendo monitorados (atualizado a cada 1–5 minutos).

— Dispositivos das sub-redes são adicionados automaticamente com o preenchimento de seus dados.

Em seguida, você pode conhecer as funcionalidades do painel na seção “HashCare”.
