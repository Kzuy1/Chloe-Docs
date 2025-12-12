---
sidebar_position: 5
---

# O que faz o Nesting1D?

## Informações:

Este script automatiza a criação de estudos de corte e otimização para formas estruturais, como perfis, tubos e barras.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-nesting-1d/img01.webp" alt="Imagem 01" />
    <figcaption>Imagem 01</figcaption>
</figure>

## Passo 01
Caso apareça a mensagem **``Perfis cujo comprimento não foi possível determinar``**, como na Imagem 02, esses itens serão considerados com comprimento de 0 mm e o cálculo deverá ser ajustado manualmente na planilha.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-nesting-1d/img02.webp" alt="Imagem 02" />
    <figcaption>Imagem 02</figcaption>
</figure>

## Passo 02
Será criada, na mesma pasta onde o modelo está salvo, uma pasta chamada NESTING1D. Nela, será possível encontrar um arquivo Excel que contém o estudo de corte e um arquivo de texto que exibe a mesma mensagem de erro descrita no <a href="#passo-01">Passo 01</a>. Note nas Imagens 03 e 04.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-nesting-1d/img03.webp" alt="Imagem 03" />
    <figcaption>Imagem 03</figcaption>
</figure>

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-nesting-1d/img04.webp" alt="Imagem 04" />
    <figcaption>Imagem 04</figcaption>
</figure>

## Passo 03 | OBSERVAÇÕES IMPORTANTES

### Obs. 1
Durante a execução do algoritmo para a realização do estudo, é considerado um acréscimo de 6 mm no comprimento das peças, representando a perda decorrente do corte realizado pela serra. Essa consideração é aplicada universalmente, exceto nos casos em que a peça possui exatamente 6000 mm de comprimento.

### Obs. 2
Peças em que é utilizada a ferramenta de revolução são consideradas com 0 mm de comprimento. Podem ser uma chapa ou um perfil.

<figure>
    <img src="/img/inventor/ilogic/o-que-faz-o-nesting-1d/img05.webp" alt="Imagem 05" />
    <figcaption>Imagem 05</figcaption>
</figure>