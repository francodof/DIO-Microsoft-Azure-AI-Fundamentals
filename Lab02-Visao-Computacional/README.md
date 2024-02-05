# Reconhecimento Facial e Transformacao de Imagens com Azure Studio Vision

<div align="center">
<img src = "https://img.shields.io/badge/microsoft%20azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white" alt = "Microsoft Azure"> 
&nbsp &nbsp &nbsp &nbsp
<img src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png" width=60 alt = "DIO">
</div>

Laboratório integrante do **Bootcamp Microsoft AI Fundamentals**, oferecido pela [Dio](https://www.dio.me/) em parceria com a Microsoft.

Realizamos configurações do Azure Studio Vision para processos automatizados de identificação facial, reconhecimento ótico de caracteres e descrições de imagens.

## Configurando o Serviço

Dentro do https://portal.azure.com/ clique em `Criar um recurso` no painel lateral. Em seguida escolha a categoria `IA + Machine Learning` e em `Serviços Cognitivos` clique em *criar*.

<img src = img-readme/01.png alt="IA + ML" width=400>

Preencha a próxima tela como na figura abaixo (apenas a aba `Noções básicas` será preenchida) e clique em `Criar`no fim da página.

<img src = img-readme/02.png alt="Serviços Cognitivos" width=400>

## Detecção de Faces

Em seguida acesse o Vision Studio em https://portal.vision.cognitive.azure.com/, vá em `My resources`e, se necessário, dê um *Refresh* para que apareça. Selecione o recurso e abaixo clique no botão `Select as default resource`.

<img src = img-readme/03.png alt="visionstudioteste as default" width=400>

Feche a página de definições selecionando o “x” no canto superior direito do ecrã. Cairá em outra tela.

Nessa tela selecione `Face` e escolha `Detects face in an image`.

<img src = img-readme/04.png alt="Detects face in an image" width=400>

Marque a caixa abaixo de `Try it out` onde é recomendada a política de uso de recursos.

Você pode selecionar cada uma das imagens de amostra e observar os dados de detecção de rosto que são retornados.

Um exemplo de imagem foi utilizado. Note 4 das faces frontais foram reconhecidas. O arquivo resultante em .json encontra-se no diretório output (detect-faces-viajantes.json).

<img src = img-readme/10.png alt="viajantes" width=400>

Feche a página clicando no "x" no canto superior direito do ecrã.

## Análise de Documentos

Selecionaremos agora a aba `Optical character recognition` e escolhendo `Extract text from images`.

<img src = img-readme/05.png alt="Optical character recognition" width=400>

Clique numa das imagens e observe como o texto é reconhecido.

<img src = img-readme/06.png alt="reconhecimento de texto" width=400>

Um exemplo de imagem foi utilizado. Note minha bela caligrafia ao estudar testes de hipóteses e, mesmo a letra sendo horrível, o modelo consegui identificar o texo do documento. O arquivo resultante em .json encontra-se no diretório output (extract-text-letrafeia.json).

<img src = img-readme/09.png alt="reconhecimento de caractere" width=400>



## Descrição de Imagens

Repita os procedimentos anteriores para fechar o ecrã e agora na aba `Image analysis` escolha `Add captions to images` para gerar uma legenda ao conteúdo da imagem. O resultado é visto abaixo. Um recurso importante em termos de acessibilidade, informando texto, por exemplo, a pessoas com deficiência auditiva.

Abaixo a inserção de nova imagem e o resultado do reconhecimento dela.

<img src = img-readme/07.png alt="descrição de imagens" width=400>

Uma imagem de joaninhas sobre uma folha também conseguiram ser identificadas e descritas pelo algoritmo, como mostrado na imagem abaixo. 

<img src = img-readme/08.png alt="Optical character recognition" width=400>


```
{
  "apim-request-id": "cf886102-fd07-4be7-8197-85b4d4d818e5",
  "content-length": "150",
  "content-type": "application/json; charset=utf-8",
  "modelVersion": "2023-10-01",
  "captionResult": {
    "text": "two ladybugs on a leaf",
    "confidence": 0.8473349809646606
  },
  "metadata": {
    "width": 1280,
    "height": 720
  }
}
```

## Referências

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html





