# Começando com ESP32 na Arduino IDE

Este tutorial apresenta, de forma simples e passo a passo, como preparar a Arduino IDE para programar placas ESP32.

---

## Objetivo

Ao final deste tutorial, você deverá ser capaz de:

- instalar ou abrir a Arduino IDE;
- adicionar o suporte às placas ESP32;
- selecionar corretamente a placa;
- identificar a porta serial;
- compilar e enviar um primeiro programa para a placa.

---

## O que você vai precisar

- 1 placa ESP32;
- 1 cabo USB compatível com transmissão de dados;
- 1 computador com a Arduino IDE instalada;
- conexão com a internet para instalar o pacote das placas.

> Atenção: alguns cabos USB servem apenas para alimentação e **não transmitem dados**.  
> Se a placa não aparecer no computador, o problema pode ser o cabo.

---

## Etapa 1 — Abrir a Arduino IDE

Abra a Arduino IDE no seu computador.

Ao iniciar, você verá a janela principal do ambiente de programação.

**Espaço para imagem/GIF:**
![Abrindo a Arduino IDE](docs/imagens/arduino-ide-abertura.gif)

---

## Etapa 2 — Abrir as preferências

No menu superior, acesse:

**File > Preferences**  
ou, em português, dependendo da instalação:  
**Arquivo > Preferências**

Nesta janela, localize o campo:

**Additional Boards Manager URLs**

É nesse campo que será informado o endereço para instalação do suporte ao ESP32.

**Espaço para imagem/GIF:**
![Abrindo as preferências](docs/imagens/arduino-ide-preferencias.gif)

---

## Etapa 3 — Adicionar a URL das placas ESP32

No campo **Additional Boards Manager URLs**, adicione a seguinte URL:

```text
https://espressif.github.io/arduino-esp32/package_esp32_index.json

## Etapa 4 — Abrir o Gerenciador de Placas

Agora vá até:

**Tools > Board > Boards Manager**  
ou  
**Ferramentas > Placa > Gerenciador de Placas**

Na caixa de busca, digite:

```text
esp32

Localize o pacote das placas ESP32, normalmente associado à Espressif Systems

Clique em Install

## Etapa 5 — Conectar a placa ESP32 ao computador

Conecte a placa ESP32 ao computador utilizando um cabo USB adequado.

> Atenção: alguns cabos USB servem apenas para alimentação elétrica e **não permitem a transmissão de dados**.  
> Se a placa não for reconhecida pela Arduino IDE, teste outro cabo antes de prosseguir.

Ao conectar a placa, observe os seguintes pontos:

- a placa pode acender um LED de alimentação;
- o sistema operacional deve detectar um novo dispositivo USB;
- a Arduino IDE poderá disponibilizar uma porta serial correspondente à placa.

Se você estiver usando Linux, é comum que a placa apareça em uma porta como:

/dev/ttyUSB0 ou /dev/ttyACM0

Se estiver no Windows, a porta geralmente aparece como: COM3, COM4, COM5

Se nada acontecer ao conectar a placa, verifique:

    se o cabo USB transmite dados;

    se a placa está corretamente conectada;

    se a porta USB do computador está funcionando;

    se o sistema reconheceu o dispositivo.

Espaço para imagem/GIF:

## Etapa 6 — Selecionar a placa correta

Depois de instalar o pacote de placas ESP32, é necessário informar à Arduino IDE qual modelo de placa será utilizado.

No menu superior, acesse:

**Tools > Board**  
ou  
**Ferramentas > Placa**

Será exibida uma lista com várias famílias e modelos de placas suportadas.

Procure a seção relacionada ao **ESP32** e selecione a placa correspondente ao seu hardware.

Em muitos casos, especialmente em atividades didáticas com placas genéricas de desenvolvimento, uma opção bastante utilizada é:

```text
ESP32 Dev Module


Se você souber exatamente o modelo da sua placa, selecione o item correspondente.
Caso não saiba, a opção ESP32 Dev Module costuma funcionar bem como escolha inicial em muitas placas ESP32 de uso educacional e experimental.

Selecionar a placa correta é importante porque essa escolha afeta parâmetros de compilação e envio do programa, como tipo de microcontrolador, velocidade de gravação e configurações internas da placa.

Se a placa errada for escolhida, podem ocorrer problemas como:

    falha no upload do programa;

    funcionamento incorreto do código;

    ausência de comunicação adequada com a placa.



