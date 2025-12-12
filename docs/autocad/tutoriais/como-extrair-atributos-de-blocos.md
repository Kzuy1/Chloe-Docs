---
sidebar_position: 2
---

# Como Extrair Atributos de Blocos?

## Informações:
- Este tutorial é aplicável tanto ao AutoCAD quanto ao AutoCAD LT;
- Cada etapa incluirá uma imagem explicativa.

## Passo 01
Digite o comando **``EXTRATRIB / ATTEXT``** na barra de comando e pressione **``Enter``**, como demonstrado na Imagem 01.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

## Passo 02
Ao acessar a aba denominada **``Extração de Atributos``**, no canto superior esquerdo dessa aba selecione a opção **``Arquivo delimitado por vírgulas (CDF)``**, como demonstrado na Imagem 02.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>

## Passo 03
Clique no botão **``Selecionar objetos``**, localizado à esquerda, na parte central, como desmonstrado na Imagem 03.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img03.webp" alt="Imagem 03" />
    <figcaption>Imagem 03</figcaption>
</figure>

## Passo 04
Selecione os Blocos Brancos, Bloco de Parafuso ou Bloco de Material que deseja como mostrado na Imagem 04.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img04.webp" alt="Imagem 04" />
    <figcaption>Imagem 04</figcaption>
</figure>

## Passo 05
Clique no botão **``Template de arquivo``**, localizado à esquerda, na parte central, como desmonstrado na Imagem 05.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img05.webp" alt="Imagem 05" />
    <figcaption>Imagem 05</figcaption>
</figure>

## Passo 06
Irá abrir a aba **``Template de Arquivo``**, onde você deverá inserir o link fornecido abaixo no campo **``Nome do arquivo``** e clicar no botão **``Abrir``**, como desmonstrado na Imagem 06.

```
L:\Drives compartilhados\EMB_ENGENHARIA_BIBLIOTECA\PADRÕES PROGRAMAS\AUTOCAD\EXTRAÇÃO
```

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img06.webp" alt="Imagem 06" />
    <figcaption>Imagem 06</figcaption>
</figure>

## Passo 07
Você encontrará quatro templates para extração. Selecione o template desejado e clique no botão **``Abrir``**, como desmonstrado na Imagem 07

Abaixo, você verá qual configuração de extração se aplica a qual bloco e os atributos que cada configuração extrai.

| Template de Extração            | Bloco que aplica           | Atributos Extraído                                       |
| ------------------------------- | -------------------------- | -------------------------------------------------------- |
| CONFIG EXTRAÇÃO                 | Bloco Branco               | Tag, Quantidade, Peso Unitário e Peso Total              |
| CONFIG EXTRAÇÃO DESCRIÇÃO-PEÇAS | Bloco Branco               | Tag, Descrição, Quantidade, Peso Unitário e Peso Total   |
| CONFIG EXTRAÇÃO - PARAFUSO      | Bloco Azul / Bloco Amarelo | Posição, Código, Descrição e Quantidade                  |
| CONFIG EXTRAÇÃO - MATERIAL      | Bloco de Material          | Posição, Descrição, Unidade, Quantidade, Material e Peso |

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img07.webp" alt="Imagem 07" />
    <figcaption>Imagem 07</figcaption>
</figure>

## Passo 08
Clique no botão **``Arquivo de saída``**, localizado à esquerda na parte central, como desmonstrado na Imagem 08.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img08.webp" alt="Imagem 08" />
    <figcaption>Imagem 08</figcaption>
</figure>

## Passo 09
Uma aba chamada **``Arquivo de Saída``** será aberta. Clique na opção **``Área de Trabalho``** para definir o local do arquivo de saída e, em seguida, clique em **``Salvar``**, como desmonstrado na Imagem 09.

Se você não definir um caminho de saída, o arquivo será salvo na mesma pasta onde o desenho está localizado

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img09.webp" alt="Imagem 09" />
    <figcaption>Imagem 09</figcaption>
</figure>

## Passo 10
Clique no botão **``Ok``**, localizado na parte inferior central, para gerar um arquivo de texto contendo as informações dos blocos, conforme demonstrado na Imagem 10. 

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img10.webp" alt="Imagem 10" />
    <figcaption>Imagem 10</figcaption>
</figure>

## Passo 11
No **``Explorador de arquivos``** insira o link fornecido abaixo, conforme demostrado na Imagem 11.

```
L:\Drives compartilhados\EMB_ENGENHARIA_BIBLIOTECA\PADRÕES PROGRAMAS\AUTOCAD\EXTRAÇÃO
```

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img11.webp" alt="Imagem 11" />
    <figcaption>Imagem 11</figcaption>
</figure>

## Passo 12
Será redirecionado para uma pasta  com **``Planilhas para Extração``**. Selecione a planilha desejada abra uma, conforme demostrado na Imagem 12.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img12.webp" alt="Imagem 12" />
    <figcaption>Imagem 12</figcaption>
</figure>

## Passo 13
Abra o arquivo de texto gerado no <a href="#passo-10">Passo 10</a> que deve estar na Área de Trabalho, selecione todo o conteúdo com **``CTRL+A``** e copie-o com **``CTRL+C``**, conforme demostrado na Imagem 13.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img13.webp" alt="Imagem 13" />
    <figcaption>Imagem 13</figcaption>
</figure>

## Passo 14
Cole os dados na célula **``A2``** da planilha para garantir que você tenha todas as informações dos blocos.

<figure>
    <img src="/img/autocad/tutoriais/como-extrair-atributos-de-blocos/img14.webp" alt="Imagem 14" />
    <figcaption>Imagem 14</figcaption>
</figure>