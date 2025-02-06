# Racks

Um **Rack** é uma entidade vinculada a uma sala específica e inclui um determinado número de espaços para dispositivos. Exibe apenas os dados dos dispositivos dentro dele.

• É possível criar um número ilimitado de racks em uma única sala.

• Por padrão, é criado um rack vinculado à sala criada.

## **Tabela "Racks"**

• **Pesquisa** — busca pelo nome.

• **Centro de Dados** — seleção de racks em um centro de dados específico.

• **Salas** — seleção de racks dentro de uma sala.

• **Adicionar novo rack** — botão para criação.

## Campos da tabela:

• **ID** — identificador no banco de dados.

• **Nome** — nome do rack.

• **Centro de Dados** — nome do centro de dados.

• **Sala** — sala à qual o rack está vinculado.

• **Edição** — configuração dos parâmetros.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

## **Criar um Rack**

1. Acesse o menu **Racks**.

2. Clique no botão **Adicionar novo rack**.

3. Na janela que aparece:

* Insira um nome no campo **Nome**.
* Defina o número de prateleiras (Altura) de 1 a 10.
* Defina o número de espaços por prateleira (Largura) de 1 a 10.
* Selecione uma sala no menu suspenso.

4. Clique no botão **Criar**.

<figure><img src="../../.gitbook/assets/image (9).png" alt="" width="345"><figcaption></figcaption></figure>

## **Editar um Rack**

1. Clique no botão de _três pontos_ ao lado do rack desejado.

2. Selecione **Editar**.

3. Faça as alterações necessárias:

* Novo nome.
* Número de prateleiras (Altura) de 1 a 10.
* Número de espaços por prateleira (Largura) de 1 a 10.
* Sala à qual o rack será vinculado.

4. Clique em **Atualizar**.

<figure><img src="../../.gitbook/assets/image (10).png" alt="" width="344"><figcaption></figcaption></figure>

## **Excluir um Rack:** <a href="#udalenie-data-centra" id="udalenie-data-centra"></a>

1. Clique no botão de _três pontos_ ao lado do rack desejado.

2. Selecione **Excluir**.

3. Na janela que aparece, clique em **Confirmar**.

<figure><img src="../../.gitbook/assets/image (11).png" alt="" width="344"><figcaption></figcaption></figure>

## **Acessar a página do Rack**

* No menu **Racks**, clique no **Nome** do rack desejado.

## **Conteúdo da página do Rack**

### **Detalhes:**

• **Tamanho**: largura × altura (por exemplo, 10×10).

• **Número de espaços**: total (largura × altura).

• **Número de dispositivos**:

* **Total** — inativos + online.
* **Online** — dispositivos que enviam dados.

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

### **Gráficos:**

**• Hashrate:**

* **Asic Hashrate** — reportado pelo dispositivo.
* **Nominal Hashrate** — especificado pelo fabricante.

**• Consumo:**

* **Asic Power** — reportado pelo dispositivo.
* **Nominal Power** — especificado pelo fabricante.

**• Dispositivos:**

* **Active Asic** — dispositivos operacionais.
* **Total Asic** — todos os dispositivos, incluindo os inativos.

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

### **Mapa do Rack**

Exibe um esquema 2D com o número de espaços definidos e os dispositivos posicionados.

• Em cada célula, são indicados:

* **Hashrate real**.
* **Temperatura máxima dos chips**.

• Características da exibição:

* Se o hashrate ou a temperatura = 0 ou excederem o limite, o texto fica vermelho.
* Para visualizar problemas atuais, é possível alternar a característica exibida no canto superior direito.

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

### **Lista de dispositivos no Rack**

Exibe os dispositivos vinculados ao rack.

• A tabela inclui:

* **ID do dispositivo** — identificador único gerado pelo sistema.
* **Modelo** — definido pelo agente ou manualmente; exibe o firmware.
* **Hashrate** — desempenho atual do dispositivo:

&#x20;     🟢 Hashrate > 0

&#x20;     🔴 Hashrate = 0 ou não definido

* **Nome do trabalhador** — composto pelo nome do pool e do dispositivo, definido pelo agente ou manualmente.
* **Endereço IP** — detectado automaticamente pelo agente ou definido manualmente.

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
