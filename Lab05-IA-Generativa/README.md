# Uso de Recursos de Reconhecimento de Texto em Imagens do Azure AI Vision Studio

<div align="center">
<img src = "https://img.shields.io/badge/microsoft%20azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white" alt = "Microsoft Azure"> 
&nbsp &nbsp &nbsp &nbsp
<img src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png" width=60 alt = "DIO">
</div>

Laboratório integrante do **Bootcamp Microsoft AI Fundamentals**, oferecido pela [Dio](https://www.dio.me/) em parceria com a Microsoft.



## Configurando o Serviço

Dentro do https://portal.azure.com/ clique em `Criar um recurso` no painel lateral. Em seguida escolha a categoria `IA + Machine Learning` e em `Serviços Cognitivos` clique em *criar*.

<img src = img-readme/01.png alt="IA + ML" width=400>

Preencha a próxima tela como na figura abaixo (apenas a aba `Noções básicas` será preenchida) e clique em `Criar`no fim da página.

<img src = img-readme/02.png alt="Serviços Cognitivos" width=400>


Em seguida acesse o Vision Studio em https://portal.vision.cognitive.azure.com/, vá em `My resources`e, se necessário, dê um *Refresh* para que apareça. Selecione o recurso e abaixo clique no botão `Select as default resource`.

<img src = img-readme/03.png alt="lab5textextract as default" width=400>

Feche a página de definições selecionando o “x” no canto superior direito do ecrã. Cairá em outra tela.

## Utilizando Imagens no Serviço Optical character recognition

Acesse a aba **Optical character recognition** e escolha **Extract text from images**

<img src = img-readme/04.png alt="service" width=400>

Utilizamos três imagens coletadas da web sob a licença Creative Commons e que foram testadas no serviço de reconhecimento ótico. As imagens encontram-se no diretório inputs e as saídas, em json, no diretório outputs.


<img src = img-readme/outputs/res-im1.png alt="service" width=400>

<img src = img-readme/outputs/res-im2.png alt="service" width=400>

<img src = img-readme/outputs/res-im3.png alt="service" width=400>

Percebe-se que no segundo exemplo de imagem reconhece com erros. Já, a terceira imagem não consegue ser feita a leitura. No mais, o reconhecimento ótico tem funcionado bem para extração de textos garrafais, de jornais, etc.


# Referências

https://aka.ms/ai900-bing-copilot

https://aka.ms/ai900-azure-openai

https://aka.ms/ai900-content-filters

https://copilot.microsoft.com/