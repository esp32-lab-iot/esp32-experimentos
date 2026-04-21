# Começando com ESP32 na Arduino IDE

Este tutorial apresenta, de forma simples e passo a passo, como preparar a Arduino IDE para programar placas ESP32.

---

## 🎯 Objetivo

Ao final deste tutorial, você deverá ser capaz de:

- Instalar ou abrir a Arduino IDE;
- Adicionar o suporte às placas ESP32;
- Selecionar corretamente a placa;
- Identificar a porta serial;
- Compilar e enviar um primeiro programa para a placa.

---

## 🛠️ O que você vai precisar

- **1 placa ESP32** (Qualquer modelo da família);
- **1 cabo USB** compatível com transmissão de dados;
- **1 computador** com a Arduino IDE instalada;
- **Conexão com a internet** para baixar os pacotes.

> ⚠️ **Atenção:** Alguns cabos USB servem apenas para alimentação e **não transmitem dados**. Se a placa não aparecer no computador, o problema pode ser o cabo.

---

## Etapa 1 — Abrir a Arduino IDE

Abra a Arduino IDE no seu computador. Ao iniciar, você verá a janela principal onde o código (sketch) é escrito.

**Caminho de acesso:**
> Menu Iniciar / Aplicativos > Arduino IDE

**Espaço para imagem/GIF:**
![Abrindo a Arduino IDE](docs/imagens/arduino-ide-abertura.gif)

---

## Etapa 2 — Abrir as preferências

Para adicionar o suporte ao ESP32, precisamos indicar à IDE onde encontrar os arquivos de instalação da fabricante (Espressif).

**Caminho de acesso:**
> **File > Preferences** (ou Arquivo > Preferências)

**Espaço para imagem/GIF:**
![Abrindo as preferências](docs/imagens/arduino-ide-preferencias.gif)

---

## Etapa 3 — Adicionar a URL das placas ESP32

No campo **Additional Boards Manager URLs**, você deve colar o link oficial do repositório de placas.

**URL para copiar:**
`https://github.io`

**Espaço para imagem/GIF:**
![Configurando a URL](docs/imagens/arduino-ide-url.gif)

---

## Etapa 4 — Instalar o pacote no Gerenciador de Placas

Agora que a IDE sabe onde procurar, vamos realizar a instalação física dos arquivos de compilação.

**Caminho de acesso:**
> **Tools > Board > Boards Manager...** (Ferramentas > Placa > Gerenciador de Placas)

No campo de busca, digite **esp32**. Localize o pacote da **Espressif Systems** e clique no botão **Install**.

**Espaço para imagem/GIF:**
![Instalando o pacote](docs/imagens/arduino-ide-instalacao.gif)

---

## Etapa 5 — Conectar a placa e identificar a porta

Conecte o ESP32 ao computador via USB. O computador deve atribuir um número de porta para a comunicação.

**Caminho de acesso:**
> **Tools > Port** (Ferramentas > Porta)

Selecione a porta que aparecer (ex: **COM3**, **COM4** no Windows ou **/dev/ttyUSB0** no Linux). Se a lista estiver cinza, verifique o cabo USB.

**Espaço para imagem/GIF:**
![Selecionando a porta](docs/imagens/arduino-ide-conexao.gif)

---

## Etapa 6 — Selecionar o modelo da placa

O último passo é informar à IDE exatamente qual modelo de ESP32 você está usando para garantir a compatibilidade.

**Caminho de acesso:**
> **Tools > Board > esp32** (Ferramentas > Placa > esp32)

Para a maioria das placas de desenvolvimento genéricas (30 ou 38 pinos), utilize a opção padrão:

**Modelo recomendado:**
`ESP32 Dev Module`

**Espaço para imagem/GIF:**
![Selecionando o modelo](docs/imagens/arduino-ide-selecao-placa.gif)

---

## ✅ Conclusão

Sua IDE agora está configurada e pronta para uso! 

---

## 📚 Referências

Para se aprofundar no assunto, consulte os materiais abaixo:

- 🌐 [Artigo Embarcados: Como programar o ESP32 na Arduino IDE](https://embarcados.com.br)
- 🎥 [Vídeo Tutorial: Configurando ESP32 no Arduino (YouTube)](https://youtu.be)
